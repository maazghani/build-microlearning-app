# Question design, feedback, and evidence

## A practical question pattern

For a source-grounded Kubernetes course:

**Card:** Kubernetes schedules containerized workloads and maintains their desired state. An inference server running inside a workload loads the model and handles inference requests. These responsibilities cooperate but belong to different components.

**Question:** Which component loads the model and performs inference?

- Kubernetes scheduler — misconception: assigning workloads to machines also executes the model.
- Inference server — correct.
- Node autoscaler — misconception: adding compute also processes requests.

**After selecting scheduler:** “The scheduler chooses where the workload runs. The inference server handles the model itself. Try the component responsible for processing the request.” Allow immediate retry.

**After a correct answer on any attempt:** “You got that right! The inference server loads and runs the model; Kubernetes keeps its workload scheduled and running.” Give corrected success equal visual weight.

**Later encounter:** “A model-serving process fails to load weights even though its pod is running. Which component's startup logs are most directly relevant?” Ground this in the actual source; do not add details never taught or sourced.

**Curiosity bridge:** “How would I tell a scheduling failure from a model-loading failure?” Include lesson context so the learner need not reconstruct it.

Write question families specific to the course. For books, use the author's concepts and distinctions; do not turn interpretive judgments into unqualified factual keys.

## Feedback states

| Event | Example language | Behavior |
| --- | --- | --- |
| Correct first try | “You got that right!” | Decorated success and explanation; continue when ready. |
| Correct after retries | “You made the connection.” | Equal success treatment and completion credit. |
| Incorrect | “This handles capacity. Look for what handles the request.” | Neutral repair and immediate retry. |
| Opens explanation | “Good move checking the explanation.” | Recognize effort without claiming correctness. |
| Reveals answer | “Now you can see the distinction.” | Record exploration; invite a nearby question, not a mastery claim. |
| Completes module | “One more set of ideas connected.” | Quiet milestone and optional curiosity bridge. |
| Returns later | “Welcome back—continue where you left off.” | Resume without a lost-streak message. |

Choose language supported by the event. A random click does not prove understanding. Keep acknowledgment light enough to avoid repetitive noise. The entire loop works with animation disabled.

## Evidence and limits

Use the recognition-first instructional approach while distinguishing empirical support from design inference.

- [McDermott et al., 2014, Both Multiple-Choice and Short-Answer Quizzes Enhance Later Exam Performance in Middle and High School Classes](https://pdf.retrievalpractice.org/guide/McDermott_etal_2014_JEPA.pdf): classroom experiments found learning benefits from quizzing with feedback, with multiple-choice and short-answer formats comparably effective under the studied conditions. This supports MCQs as a serious teaching interaction, not universal equivalence across tasks. It does not isolate decorative praise or unlimited retries as causal factors.
- [Mayer, Pre-training Principle](https://www.cambridge.org/core/books/abs/multimedia-learning/pretraining-principle/01791D57F5D4164251269E6DF56A8BF1): introduce component names/characteristics before complex multimedia explanations. Apply as gradual foundational vocabulary, not a mandatory wall of definitions or a proven requirement for exactly 5–12 terms.
- [Loewenstein, The Psychology of Curiosity: A Review and Reinterpretation](https://www.cmu.edu/dietrich/sds/docs/loewenstein/PsychofCuriosity.pdf): the information-gap account motivates helping learners notice questions they can articulate. The AI bridge is our design application; this older theory is not an AI-tutoring trial.

Consult the original sources before making stronger efficacy claims. Do not portray the whole recipe, exact timings, three-question recurrence, or motivational decoration as a validated experimental intervention. These are practical design defaults.

MCQs can themselves involve retrieval. Do not force that terminology debate into the app or replace the chosen interaction with free-response testing. Evaluate clearer distinctions, contextual application, continued participation, and better questions.
