# Example: Rank What Matters

**Course:** MTH 266 Linear Algebra
**Subject matter:** Eigenvalues and eigenvectors, Markov chains, stochastic matrices
**Professor notes:** Mixed online and in-person sections, two to three weeks, students have free AI tools and Python or a spreadsheet

This is the worked example from the talk. It is one of the three options the skill would draft, shown here in full.

## The challenge

Choose 10 to 20 things you can compare head to head: sports teams, local restaurants, courses, songs, video games, hiking trails. Build a ranking of them from a Markov chain and its dominant eigenvector, the same idea behind Google's PageRank.

Use any AI tool you like, for exploring approaches, writing code, explaining concepts, or checking your work. You decide what "better" means, and you defend it.

## The open decision (the student's loss function)

There is no answer key. Each student decides:

- What a head-to-head "win" means. Does a win by 20 count more than a win by 1? Does a 5-star review beat a 4-star review, and by how much?
- How to turn those wins into transition probabilities.
- How to handle ties, missing matchups, and items that never "win."
- Whether to add a damping factor, and why.

## Deliverables

1. **The ranking, the matrix, and code they verified.** Show that the matrix is column-stochastic and that the vector really is an eigenvector for eigenvalue 1.
2. **A decision log.** Every modeling choice, the alternatives considered, and why this one.
3. **An annotated AI log.** Where it helped, where it was wrong, and how they caught it. See `templates/ai-use-log.md`.
4. **A stress test.** Change one assumption, show what moves in the ranking, and explain why.
5. **A three-minute defense.** Live, or recorded for online sections. Explain the ranking to someone who has never taken linear algebra, then take two questions.

## Milestones

| Day | Check-in |
|---|---|
| 3 | Items chosen, data source identified, definition of a "win" drafted |
| 8 | Matrix built and verified as stochastic; first ranking computed |
| 12 | Stress test done; AI log at least half complete |
| 15 | Final submission and defense |

## Scaffolding (for students who are stuck)

- Start with four items you can rank by hand. Build the 4×4 matrix and check that the eigenvector agrees with your intuition.
- If your chain has an item with no outgoing links, ask yourself what a random visitor would do there.
- If your ranking looks wrong, check your column sums before you check your code.

## Stretch

Compare your eigenvector ranking with a simple win-percentage ranking. Where do they disagree, and which one would you trust? Why?

## Why copying won't work

The data choice is personal, the definition of a win is the student's own, the stress test depends on their specific model, and the defense requires them to explain their choices live. An AI can help with every step, but it can't make the decisions for them.

## Rubric (100 points)

### What they arrived at (40)

| Criterion | Exemplary | Proficient | Developing | Beginning |
|---|---|---|---|---|
| **Mathematical correctness (15)** | 14–15: Matrix is verified stochastic; eigenvector is verified (Av = v) independently of the code that produced it; no errors | 11–13: Correct, with verification for most steps; minor slips that don't affect the ranking | 7–10: Mostly correct, but verification is missing or one error changes the ranking | 0–6: Matrix or eigenvector is wrong, or no verification |
| **Fit to the question (15)** | 14–15: The ranking clearly answers the question they framed; the model's choices follow from that framing | 11–13: Ranking answers the question; one or two choices aren't connected to the framing | 7–10: Ranking and framing only loosely connected | 0–6: No clear question, or the ranking doesn't address it |
| **Originality (10)** | 9–10: A domain, data set, or modeling choice that's genuinely their own and produces an insight | 7–8: Their own domain with a standard model | 4–6: A common example with little adaptation | 0–3: Reproduces a tutorial or example |

### How they got there (60)

| Criterion | Exemplary | Proficient | Developing | Beginning |
|---|---|---|---|---|
| **Problem framing (15)** | 14–15: Defines "better" precisely, names alternatives, states every assumption and its consequence | 11–13: Clear definition and most assumptions stated | 7–10: Definition stated but not justified; assumptions implicit | 0–6: No definition of "better" |
| **Verification (15)** | 14–15: Independent checks at each stage; documents at least one AI or code error they caught and how | 11–13: Checks key results; notes where AI output needed correction | 7–10: Some checking, mostly at the end | 0–6: Takes outputs on faith |
| **Iteration (10)** | 9–10: Log shows the approach changed for a stated reason, more than once | 7–8: At least one meaningful revision, explained | 4–6: Revisions happened but aren't explained | 0–3: Single pass |
| **Purposeful tool use (10)** | 9–10: AI log is honest and specific; uses AI deliberately for different jobs and says why | 7–8: Clear, honest log with some reflection | 4–6: Log is thin or generic | 0–3: No log, or use not disclosed |
| **Communication and defense (10)** | 9–10: A non-mathematician would understand the ranking; answers questions with confidence and precision | 7–8: Clear explanation; handles most questions | 4–6: Explanation relies on jargon; struggles with questions | 0–3: Cannot explain own choices |

### The same rubric, for students

- **Is it right?** Your matrix and eigenvector check out, and you proved it without just trusting your code.
- **Does it answer your question?** Your ranking answers the question you asked, and your choices follow from that question.
- **Is it yours?** You picked something you care about and made it your own.
- **Did you define "better"?** You said exactly what wins mean and what you assumed.
- **Did you check it?** You caught mistakes, including the AI's, and wrote down how.
- **Did you revise?** Your log shows you changed course when you learned something.
- **Did you use your tools well?** Your AI log is honest and specific.
- **Can you explain it?** Someone who's never taken linear algebra could follow you.
