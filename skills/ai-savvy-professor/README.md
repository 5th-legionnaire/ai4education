# AI-Savvy Professor

A free tool for faculty who want to design assignments for a world where students have AI.

You give it a course, a topic, and your notes. It drafts three open-ended "Math++" challenges in which students use AI as part of the work and create something new. It also drafts a rubric that grades both **what students arrived at** and **how they got there**, plus a student handout and an AI-use log.

You review it, adapt it, and own the result. You stay the one who writes the loss function.

## Why

A correct answer to a rote problem is now easy to get. What's worth grading is how a student navigates a hard, open problem: how they frame it, check it, iterate on it, use their tools, and what they create.

Students optimize against a rubric the way a model optimizes against its loss function. Change the rubric and you change what they learn to do.

## What's here

| File | What it is |
|---|---|
| `SKILL.md` | The skill itself. Works as a Claude skill, or as a prompt you paste into any AI assistant. |
| `PROMPT.md` | How to use it with ChatGPT, Gemini, Copilot, or anything else. |
| `examples/mth266-rank-what-matters.md` | A complete worked example for Linear Algebra, with a full rubric. |
| `templates/ai-use-log.md` | A log students fill in as they work. |

## Using it with Claude

Add this folder as a skill in Claude (it contains `SKILL.md`), then ask something like: "Use the AI-Savvy Professor to design a challenge for MTH 265, Lagrange multipliers, online section, two weeks."

## Using it with anything else

See `PROMPT.md`.

## The rubric, at a glance

| What they arrived at (40) | How they got there (60) |
|---|---|
| Mathematical correctness (15) | Problem framing (15) |
| Fit to the question they framed (15) | Verification (15) |
| Originality (10) | Iteration (10) |
| | Purposeful tool use (10) |
| | Communication and defense (10) |

Change the weights to fit your course.

## About

Built by Josh Latz for a talk at the NOVA Mathematics Community of Practice, October 16, 2026. Feedback, improvements, and examples from your own courses are welcome. Open an issue or a pull request.

## License

Apache 2.0, same as the rest of this repository. Use it, change it, share it.
