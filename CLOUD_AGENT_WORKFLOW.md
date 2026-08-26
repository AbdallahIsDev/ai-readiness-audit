# CLOUD AGENT WORKFLOW — REFERENCE

This file describes the execution environment and operating model that any idea from `IDEA_DISCOVERY_PROMPT.md` must be executable through. Any agent reasoning about idea feasibility should treat this as ground truth for "what is actually buildable here."

## 1. Environment

- A cloud AI agent runs inside an online sandbox (Linux/Debian).
- The sandbox has a built-in terminal with real shell access.
- The agent can read and write files inside the sandbox.
- The agent has built-in browser control — it can operate a real browser to carry out tasks the way a human would (navigate, click, fill forms, extract data), just faster and more consistently.
- The agent has access to a broader tool library beyond the terminal and browser (exact tools vary by setup — treat "it has a capable general tool belt" as the assumption, not a fixed list).
- On completion, the agent packages all deliverables (code, reports, assets, anything requested) into a zip file placed in a download folder, which is then retrieved to the local device.

## 2. Sub-agents

- The cloud agent can launch a configurable number of sub-agents to work in parallel.
- Sub-agents inherit the same general capabilities (terminal, file I/O, browser control) and are given a specific slice of the overall task.

## 3. The Wave System

Work is organized into **waves**. A wave is a batch of sub-agents launched at the same time; waves run one after another, not concurrently with each other.

```
controls:
  SUB_AGENTS_PER_WAVE: 10   # how many sub-agents launch together in one wave
  NUM_WAVES: 4              # how many waves run in sequence
```

With the example values above: 10 sub-agents per wave × 4 waves = 40 sub-agents total across the run, executed in 4 sequential batches.

**Wave roles alternate in a fixed pattern:**

- Odd waves (1st, 3rd, ...): **Implementation** — sub-agents build/execute the assigned work.
- Even waves (2nd, 4th, ...): **Review** — sub-agents check the immediately preceding implementation wave's output: did it get done correctly, what did it miss, what needs fixing.

So with `NUM_WAVES = 4`: Wave 1 = Implementation, Wave 2 = Review (of Wave 1), Wave 3 = Implementation, Wave 4 = Review (of Wave 3). This strict alternation exists so mistakes get caught inside the run itself, before the session ends or the orchestrating agent stops — nothing ships without a review pass behind it.

Every numeric parameter of this system (`SUB_AGENTS_PER_WAVE`, `NUM_WAVES`) is configurable per task and should be tuned to the scope of the specific job, not treated as fixed.

## 4. What this means for idea feasibility

An idea is a good fit for this workflow if:

- It can be decomposed into parallelizable units of work a wave of sub-agents can each take a slice of (e.g. "research N sources," "generate N assets," "draft N pages," "scrape N sources," "test N variants").
- Its build-and-launch phase is front-loaded — heavy setup/build via waves, followed by comparatively light, occasional human decision-making — rather than requiring constant real-time manual operation to run day to day.
- It doesn't require infrastructure, legal status, or capital the sandbox + human clearly don't have.

An idea is a poor fit if it fundamentally requires one continuous human-operated process with no clear way to batch or parallelize the work, or requires ongoing infrastructure/maintenance that can't be handled by occasional agent runs plus light human oversight.
