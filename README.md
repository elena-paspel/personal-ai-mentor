# Personal AI Mentor

A research prototype of a Socratically scaffolded Personal AI Mentor for adult learners. The mentor asks questions instead of giving answers, moves with the learner through a cycle of experience, reflection, concept and action, and leaves the learner with a record of their own thinking that they keep and control.

The prototype implements the conceptual architecture published in:

> Paspel, E. (2026). A Socratically scaffolded Personal AI Mentor for postdigital lifelong learning: An evidence-informed conceptual architecture. *Andragoška spoznanja/Studies in Adult Education and Learning, 32*(2), 133–155. https://doi.org/10.4312/as/27789

**Status: research prototype, version 0.7. It has been desk-tested with scripted conversations and has not yet been evaluated with learners.**

## Why it exists

AI systems are entering adult education faster than adult learning theory is entering AI design. The article argues that an AI mentor for adults needs an andragogical architecture, and specifies one with six components. Its conclusion names the next step: prototyping and empirical validation. This repository is that first prototype, built so that the design can be inspected, criticised and tested by others.

The aim is not to reproduce human mentorship. It is to design AI support that preserves learner agency, supports reflective inquiry, sustains continuity across interruptions, and connects learners to the human communities that adult education depends on.

## What is in this repository

| Item | What it is | For whom |
| --- | --- | --- |
| [`mentor-instructions.txt`](mentor-instructions.txt) | The instruction set that turns a general AI chat assistant into the mentor. Paste it as the first message of a new chat. | Any learner, with any AI assistant |
| [`index.html`](index.html) | A companion page that hands over the instructions, shows the stages, and keeps the learner's dialectic trace in their own browser. | Learners; reviewers who want to try it |
| [`skill/personal-ai-mentor/SKILL.md`](skill/personal-ai-mentor/SKILL.md) | The same instructions packaged as an agent skill. | Assistants that load skills |
| [`docs/design-rationale.md`](docs/design-rationale.md) | Every rule traced to its theoretical source and to the article's tables. | Researchers, reviewers |
| [`docs/testing.md`](docs/testing.md) | Formative desk testing: method, results, failures, fixes, limits. | Researchers, reviewers |
| [`docs/transcripts/`](docs/transcripts) | The test conversations. | Researchers, reviewers |
| [`docs/CHANGELOG.md`](docs/CHANGELOG.md) | Versions 0.1 to 0.7 and the design decision behind each change. | Researchers |
| [`docs/notion-templates.md`](docs/notion-templates.md) | Two Notion templates that offer the same support without a web page. | Learners who use Notion |

## Try it

1. Open [`mentor-instructions.txt`](mentor-instructions.txt) and copy all of it.
2. Paste it as the first message in a new chat with an AI assistant.
3. Answer the mentor's first question. Type `pause` when you want to stop; the mentor shows your trace. Save it.
4. Next time, paste the instructions again, followed by your saved trace.

The companion page does steps 1 and 4 with one button and keeps the trace for you. It is live at https://elena-paspel.github.io/personal-ai-mentor/

## The design in brief

The article specifies six architecture components. The prototype realises them as follows.

| Component | In the prototype |
| --- | --- |
| Goal-oriented engagement | Every session opens with the learner's own purpose. A learner without a clear goal is not pressed for one; finding the question is treated as the work of the session. |
| Socratic-Kolb process | Four stages after the goal: experience, reflection, concept, action. In each, the mentor takes a named role (Facilitator, Provocateur, Subject Expert, Coach) and asks one category of Socratic question. |
| Dialectic trace | A twelve-line record in the learner's words. The learner can see it, correct it and take it away. The learner's version stands. |
| Resilient continuity | The trace carries the central question, the surfaced assumption and the planned experiment into the next session. The mentor has no hidden memory or profile. |
| Human bridge | Six triggers route a question to people. The mentor names the limit of its reasoning and prepares a hand-over for a peer, mentor, supervisor or community. |
| Agentic constraints | Eight rules that always hold, such as learner agency before system autonomy and depth before speed, plus safeguards on disclosure, assessment, profiling and privacy. |

Three behaviours distinguish the mentor from a general assistant. Whether it answers depends on the kind of question, never on how hard the learner insists: a needed fact gets a brief clarification, a judgement does not get a verdict. It does not write, score or approve the learner's work. And it does not confirm that the learner is right; it asks how they would check.

## Theoretical grounding

The design rests on Dewey's pragmatism and transactional realism, and integrates andragogy (Knowles), transformative learning (Mezirow), critical inquiry (Brookfield), Socratic questioning (Paul and Elder), experiential learning (Kolb and Kolb) and social sustainability. Its evidence base is a qualitative evidence synthesis of seven studies of digital and e-mentoring in adult and professional learning. [`docs/design-rationale.md`](docs/design-rationale.md) shows which rule comes from which source, and marks where the prototype goes beyond the article.

## Evidence so far, and its limits

The instructions were revised through six rounds of formative desk testing. Scripted learners (one with no clear goal, one demanding quick answers, one facing an ethical dilemma, one returning after three weeks, and others) were run against a fresh AI assistant that had seen only the instructions. Failures in early versions led to the rules described above. Details are in [`docs/testing.md`](docs/testing.md).

This is not evidence about real learners. Each scenario was run once, on one AI assistant, with scripted learner turns. Whether the design preserves agency, deepens reflection or transfers to practice for actual adults is the question the planned research is meant to answer.

## Planned research

1. **Pilot with adult learners** across varied professional contexts, with measures beyond technical accuracy: preserved learner agency, reflective depth, transfer to practice, accessibility, and the quality of escalation to human community.
2. **An engineered prototype** that replaces copy and paste with an integrated interface, and connects to learning platforms used by European institutions.
3. **Governance work** on data protection and on the EU AI Act, which treats AI systems used to assess or evaluate learners as high-risk. The mentor is designed not to assess learners.

## Safeguards and boundaries

The mentor states that it is an AI. It does not grade, score, rank or profile learners. It asks learners not to share names or confidential information. The companion page stores the trace only in the learner's browser and sends nothing anywhere; text pasted into an AI assistant goes to that assistant's provider. This prototype is not a substitute for professional, medical or legal help.

## Use of generative AI

The architecture, the design decisions and the resolution of every test failure are the author's. An AI assistant (Claude, Anthropic) was used to draft the instruction text, the companion page, the Notion templates and this documentation, and to run the scripted test conversations, under the author's direction. The version history records which decision led to which change.

## How to cite

Please cite the article above. To cite this prototype specifically:

> Paspel, E. (2026). *Personal AI Mentor: mentor instructions and companion* (version 0.7) [Research prototype]. https://github.com/elena-paspel/personal-ai-mentor
>
> Author ORCID: https://orcid.org/0009-0008-9306-7058

Citation metadata is in [`CITATION.cff`](CITATION.cff).

## Licence

Text, instructions and documentation: CC BY-SA 4.0. Code of the companion page: MIT. See [`LICENSE.md`](LICENSE.md).
