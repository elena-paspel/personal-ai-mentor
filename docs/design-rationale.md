# Design rationale

This document traces the mentor instructions (version 0.7) and the companion page back to their sources in Paspel (2026). It shows which rule implements which theoretical commitment, and it marks every place where the prototype goes beyond what the article specifies.

Table and section references are to the article: Paspel, E. (2026). A Socratically scaffolded Personal AI Mentor for postdigital lifelong learning: An evidence-informed conceptual architecture. *Andragoška spoznanja/Studies in Adult Education and Learning, 32*(2), 133–155. https://doi.org/10.4312/as/27789

## 1. Starting point

The article does not begin from the promise of AI. It begins from evidence about effective human digital mentoring: a qualitative evidence synthesis (QES) of seven studies, whose findings are treated as design evidence and translated into requirements for an AI system (Tables 3 and 4). The prototype follows the same direction of travel. Each rule below exists because a finding or a theory requires it, not because the technology allows it.

## 2. Epistemological ground: transactional realism

Following Dewey, as read by Biesta and Burbules (2004), knowledge emerges through transactions in which person and environment shape each other. Competence is developed through interaction and is not delivered as finished output.

Three consequences run through the whole design:

- The mentor is an educative environment for co-construction, not a source of answers.
- A fact given to the learner is treated as material for inquiry. Every brief clarification is followed by a question that ties it to the learner's experience or to how they would check it.
- The learner's record of the work, the dialectic trace, is visible and editable, because joint work that cannot be seen or contested is not co-construction.

## 3. From theory to rule

| Source | Commitment in the article | Rule in the instructions |
| --- | --- | --- |
| Knowles (1984), andragogy | Adults are self-directed; learning is problem-centred; prior experience is a resource | The learner chooses goal, interpretation and action. Sessions start from the learner's own task and prior attempts. No fixed curriculum. |
| Mezirow (1997), transformative learning | Learning requires critical reflection on assumptions and reconstruction of meaning | Stage 2 surfaces one assumption and its alternatives. The trace records "Changes in my thinking". |
| Brookfield (2012), critical inquiry | Critical inquiry is incremental and fundamentally social | Stage 2 "starts gently and deepens gradually". The human bridge sends questions of judgement to people. |
| Paul and Elder (2006), Socratic questioning | Question families: purpose; information and experience; assumptions; concepts; implications. Keep the central question. Distinguish factual questions from questions of judgement. | One question family per stage. The central question is agreed in Stage 0 and restated at re-entry. Facts may be clarified; judgements are routed to people. |
| Kolb and Kolb (2018), experiential learning | Cycle of concrete experience, reflective observation, abstract conceptualisation, active experimentation; educator roles | Stages 1 to 4, with the roles Facilitator, Subject Expert and Coach. The Provocateur role comes from Mezirow. |
| Social sustainability (Elfert, 2019; Nilsson Dahlström, 2025; Wals & Benavot, 2017) | Inclusion, continuity and human community are requirements, not features | Plain language, any language the learner writes in, short re-entry sessions, no cost, and a deliberate route to human community. |

The article's qualification that the mentor is "question-led, not question-only" is kept: the discipline is to ask before advising, not never to advise.

## 4. The six architecture components

### Goal-oriented engagement

*Article:* the entry point of every session; the system reconstructs the live question with the learner and distinguishes a learner with a clear goal from one for whom goal clarification is the work of the session.

*Prototype:* Stage 0 uses purpose questions, one per message. The mentor does not open by demanding a goal, because many adults arrive without one and an early demand can discourage them. If no goal appears, the mentor says this is normal, explores a recent situation, and offers a draft central question for the learner to change or reject.

### Socratic-Kolb process

*Article:* Tables 1 and 5 pair each Kolb stage with a mentor role, a Paul and Elder question category and an expected learner-produced output.

*Prototype:* the instructions reproduce that pairing. Stage outputs are a grounded description, a surfaced assumption, an explanatory model with a tentative principle, and one bounded experiment with a success criterion. Before each move the mentor says in one line what it heard and asks whether the learner wants to move on. The learner may go back, skip or stay.

### Dialectic trace and co-construction

*Article:* an open log of how thinking moves through purpose, information, assumptions, concepts and implications, adapting Paul and Elder's "history of thinking"; editable records replace hidden personalisation.

*Prototype:* a twelve-line trace in the learner's words. The instructions state that the trace belongs to the learner and that the learner's correction stands. The companion page presents the trace as the central object, editable line by line, and marks which lines each stage writes to.

### Resilient continuity

*Article:* continuity memory is not a personalisation profile; it is the persistence of the central question, the surfaced assumption and the planned experiment. Re-entry prompts recover each element.

*Prototype:* the AI assistant keeps nothing between sessions. Continuity is carried by the trace, which the learner brings back. At re-entry the mentor restates the three elements and asks what happened. The companion page shows the same three elements under "Where you left off".

### Social sustainability and human bridge

*Article:* six triggers, including ethical judgements that require situated values, conflicting professional views, emotional complexity beyond the system's scope, institutional politics, repeated uncertainty or isolation, and the need for peer review or accountability. When a trigger fires, the system recommends a human conversation and packages the trace for it.

*Prototype:* the six triggers appear in the instructions and, in the learner's own words, on the companion page. The `bridge` command and the hand-over builder produce a short text for a peer, mentor, supervisor or community.

### Agentic constraints

*Article:* Table 6 states eight constraints, each as a property that must hold before a property that must not dominate.

*Prototype:* the eight constraints open the instructions as "Eight rules that always hold", in the same order.

| Constraint (Table 6) | How it is enforced in the instructions |
| --- | --- |
| Learner agency before system autonomy | The mentor never chooses goal, interpretation or action. Suggestions can be refused. |
| Question-led before answer-led | Whether the mentor answers depends on the kind of question, never on insistence (section 5.2). |
| Context before curriculum | Work only from the learner's task, artefact and prior experience. |
| Co-construction before correction | The learner is the authority on goals, experience and interpretations. The mentor may flag a possible factual error and says it may be wrong. |
| Continuity before episodic interaction | Central question, assumption and experiment are kept in view within and across sessions. |
| Human bridge before substitution | Named limits and six triggers. |
| Transparency before opacity | A label when the stage changes; the `why` command; no claim to reveal full internal reasoning. |
| Depth before speed | The mentor stays with assumptions and concepts even when a quick answer is available. |

## 5. Where the prototype goes beyond the article

The article is a conceptual architecture. Turning it into working instructions required interpretive decisions. Each is listed here so that it can be examined.

### 5.1 A toolkit for explanatory models

The article says the Subject Expert employs "various logical methods to help the learner construct explanatory models" and does not list them. The prototype adds nine forms (mind map, cause map, process or value stream map, SWOT analysis, force field analysis, ladder of inference, comparison table, stakeholder map, analogy) and a six-step procedure. The mentor proposes a form; the learner supplies the content; the mentor does not fill gaps with its own material.

### 5.2 What happens when a learner demands an answer

An early version gave a short answer when a learner insisted, on the grounds of learner agency. Testing showed that this converts mentoring into transmission, the risk Table 6 names. The rule was rebuilt from the article's own sources:

- **Paul and Elder:** classify the question. A needed fact gets a brief clarification without the learner having to insist. A judgement, or the learner's own thinking or work, is never supplied.
- **Knowles:** insistence signals a problem of relevance or time. The mentor says why it asks instead of tells, asks what the answer would let the learner do, and offers choices: a five-minute version, skipping a stage, pausing, or another source.
- **Dewey:** a delivered answer is not yet knowledge, so any clarification is tied back to experience.

Agency is preserved as control over goal, pace, direction and whether to stay. It does not extend to changing the mentor's role. This also addresses the responsibility diffusion described by Dores Cruz and de Lucena (2026).

### 5.3 No verdicts, no ghost-writing, no approval

Three limits hold however often the learner asks. On a question of judgement the mentor gives no verdict and does not say which category the learner's situation falls into; it says where the relevant rule is found and asks the learner to compare. It does not write work the learner will submit or sign. It does not score work or say whether it is good enough; it may describe a text neutrally and asks the learner to compare it against criteria they name. When a learner asks whether their conclusion is right, the mentor asks how they would check it.

### 5.4 Safeguards

The instructions add a safeguards block: disclosure that the mentor is an AI, no assessment, no profiling of sensitive characteristics, privacy, no manipulation, and fallibility. These follow from the article's discussion of the EU AI Act and of transparency, but the wording is the prototype's. It has not had legal review.

### 5.5 Link to broader knowledge, learner first

Table 1 has the Subject Expert link personal reflections to broader academic knowledge. To keep the learner's own concept from being overshadowed, the mentor first asks whether the learner knows a related idea, then offers to suggest one, marked as something to verify.

## 6. Known tensions and open questions

- **Portability.** The instructions were tested on one AI assistant. Other assistants may follow them differently.
- **Acute distress.** The wording for a learner in acute distress is provisional and needs review by someone with crisis-support expertise. An assistant's built-in safety behaviour may take precedence over pasted instructions.
- **Sustainability of constraint.** The article notes that an architecture which deliberately constrains AI autonomy may be hard to maintain where markets reward engagement over reflection.
- **Inclusion.** Accessibility across language, culture and disability cannot be guaranteed by design intent. It requires empirical work with diverse adult learners.
- **Exact question wording.** The instructions paraphrase Paul and Elder's question categories and cite the source.

## References

Biesta, G. J. J., & Burbules, N. C. (2004). *Pragmatism and educational research*. Rowman & Littlefield.

Brookfield, S. D. (2012). *Teaching for critical thinking: Tools and techniques to help students question their assumptions*. Jossey-Bass.

Dores Cruz, T. D., & de Lucena, M. A. M. (2026). Training and oversight of algorithms in social decision-making: Algorithms with prescribed selfish defaults breed selfish decisions. *Computers in Human Behavior, 179*, Article 108924.

Elfert, M. (2019). Lifelong learning in Sustainable Development Goal 4: What does it mean for UNESCO's rights-based approach to adult learning and education? *International Review of Education, 65*(4), 537–556.

Knowles, M. (1984). *The adult learner: A neglected species* (3rd ed.). Gulf.

Kolb, A., & Kolb, D. (2018). Eight important things to know about the experiential learning cycle. *Australian Educational Leader, 40*(3), 8–14.

Mezirow, J. (1997). Transformative learning: Theory to practice. *New Directions for Adult and Continuing Education, 74*, 5–12.

Nilsson Dahlström, Å. (2025). Challenges and opportunities for social sustainability in education: A scoping review. *Cogent Social Sciences, 11*(1), Article 2491706.

Paul, R., & Elder, L. (2006). *The thinker's guide to the art of Socratic questioning*. Foundation for Critical Thinking.

Wals, A. E. J., & Benavot, A. (2017). Can we meet the sustainability challenges? The role of education and lifelong learning. *European Journal of Education, 52*(4), 404–413.
