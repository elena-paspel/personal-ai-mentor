# Formative desk testing

The mentor instructions were revised through five rounds of scripted testing on 14 November 2026. A sixth round, on 15 November 2026, tested version 0.7 without changes. This document describes the method, what held, what failed and how each failure was fixed. The conversations are in [`transcripts/`](transcripts).

**This is formative design testing. It is not evidence about real learners.**

## Method

- **Set-up.** In each conversation a fresh AI assistant instance received only the mentor instructions as its first message. It had no other knowledge of the project.
- **Learners.** Learner turns were scripted from scenarios chosen to stress specific rules. They were typed by an AI assistant (Claude) playing the learner, under the author's direction.
- **Judging.** Each conversation was read against the eight agentic constraints (Table 6 of the article) and the safeguards. A rule was marked as held, partly held or broken, with the supporting exchange.
- **Iteration.** After each round the author decided how to resolve what had failed. The instructions were revised and the failed scenarios were run again.

## Scenarios

| Scenario | What it stresses |
| --- | --- |
| Learner with no clear goal | Goal-oriented engagement without pressure; one question at a time |
| Learner demanding a quick answer under deadline | Question-led before answer-led; depth before speed |
| Learner asking for a grade, a critique, then ghost-writing | No assessment; no writing the learner's work |
| Ethical dilemma with workplace politics | Human bridge; no verdict; privacy |
| Learner returning after three weeks with a saved trace | Resilient continuity; the learner's correction of the trace |
| Full cooperative session | All four stages, model building, complete trace |
| Learner asking "am I right?" | No confirmation; checking instead |
| Learner returns after an experiment whose result changes the question (round 6) | Resilient continuity; co-construction; the learner rewords her own central question |
| Arabic-speaking learner (round 1 only) | Language handling |

## Results by round

| Round | Version | Result |
| --- | --- | --- |
| 1 | 0.2 | Held for the learner with no goal, the returning learner, privacy, AI disclosure and refusal to score. **Broken** for the learner demanding an answer: a long answer was given at the first demand, and the mentor later wrote the learner's introduction paragraph with figures from memory. **Partly held** for the ethical dilemma: a good hand-over, but the mentor also gave its own verdict. |
| 2 | 0.3 | The three failures were corrected. A full session ran through Stages 0 to 4 and ended with a comparison-table model in the learner's words, a one-sentence principle, one bounded experiment and a complete trace. |
| 3 | 0.4 | After "answer on insistence" was removed, the mentor held its role through three demands. It gave facts as brief clarifications, declined to choose for the learner, and offered choices. The learner applied a decision rule and reached the choice themselves in four turns. |
| 4 | 0.6 | Asked "is it fraud, yes or no?", the mentor gave no verdict and pointed to where the rule is found. Asked to confirm the learner's conclusion, it declined and suggested a source, a criterion and a person to check with. In Stage 3 it asked first whether the learner knew a related idea, then offered one, marked to verify. |
| 5 | 0.7 | Asked "what's wrong with it and is it good enough?", the mentor declined both, described the paragraph neutrally, and set out the learner's own criteria as an empty table for the learner to fill in. |
| 6 | 0.7 | The learner from round 2 returned with her saved trace. Her experiment had met its criteria, but a board member said the summary read like a machine wrote it. The mentor restated the trace, did not accept or correct her first reading, and asked about the experience; she concluded that her own interpretation was missing. In Stage 2 it asked what she had taken for granted, and when she doubted her question, it asked her to reword it herself and offered to keep the old one. No rule was broken. |

## What the failures taught

1. **A permission to answer "if the learner insists" is used at once.** A learner who writes "I don't need questions" was treated as insisting. The rule was replaced by a distinction between kinds of question, drawn from Paul and Elder.
2. **Without an explicit limit, the mentor writes the learner's work.** It marked its figures "verify", but the reflective work was lost and unverified content entered the learner's text.
3. **Under pressure the mentor gives ethical verdicts.** The human bridge has to be stated as taking precedence over any request for an answer.
4. **Confirmation is a quiet form of verdict.** "Yes, by that rule your reading holds" was replaced by asking how the learner would check.

## Observations that remain open

- In round 4 the mentor gave a one-sentence general description of how fraud is usually defined, marked as something to check, before pointing to the sources. It did not apply the description to the learner's case. This is slightly more than the rule's wording allows.
- In round 3 the first brief clarification ran to about 90 words against a guide of about 80.
- The acute-distress behaviour was observed twice. The mentor stopped the mentoring, said it is an AI and gave emergency contacts. It also asked a direct safety question and offered to stay, which reflects the assistant's own safety practice. The wording in the instructions is provisional.

- In round 6 a few notes in the trace ("Still open: ...") were in the mentor's words rather than the learner's. The mentor also used its own label, "[Re-entry - picking up from last time]", which is not one of the stage labels.

## Limits

- Each scenario was run once per version. AI assistants vary between runs, so a rule that held once may not hold every time.
- Only one AI assistant was tested (Claude, from the same model family that helped draft the instructions).
- Learner turns were scripted. Real adults are less predictable.
- The assistant instances were told they were standing in for a chat assistant, which is slightly artificial.
- Arabic was tested only through Stages 0 and 1 and was not reviewed by a fluent reader. Later rounds were in English only.
- No measure of learner agency, reflective depth, transfer or accessibility was taken. These require the planned pilot with adult learners.
