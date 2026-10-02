---
name: build-microlearning-app
description: Create or improve modern, mobile-friendly microlearning web apps from researched topics, PDFs, books, or documents. Use for interactive courses and micro-labs with progressive multiple-choice learning, unlimited retries, encouraging feedback, saved progress, and optional AI exploration.
---

# Microlearning App Builder

Build a working learning experience that establishes vocabulary, sharpens distinctions, and gives learners confidence to ask better questions. Use multiple choice as the primary teaching interaction. Make entry easy and grow toward judgment without turning the course into an exam.

## 1. Establish the brief

Use information already supplied. Ask only for missing choices, in one short intake where possible. These are creator questions in the conversation, not a required onboarding form in the finished app.

- **Topic:** “What topic should the app teach?” Accept a concept, goal, or attached book/document. Infer a clear topic from the request or attachment. Clarify materially ambiguous scope rather than inventing it.
- **Sources, when documents are supplied:** “Should the supplied documents be the sole source of course content, or should I add research?” Offer **Documents only** and **Documents + research**. Preserve an existing choice. With no source documents, assume research and say so briefly; skip the source question. If the document-source question goes unanswered, default to documents only. Treat a URL as a supplied source when the user designates it as the course basis.
- **Audience:** “Who is this for?” Offer **Myself**, **Someone else**, and a **custom answer** path. If the question widget provides free-form Other, use that for custom answers instead of a duplicate choice. If Someone else supplies no useful detail, ask for their role, topic familiarity, and goal in one short follow-up. Do not require their name or ask again when the audience is explicit.

Use an available question widget for choices and plain text for a free-text topic when needed. If no answer arrives, proceed with the audience information supplied in the request; otherwise assume an introductory general audience. State the assumption. If no topic can be identified, ask for it instead of choosing an arbitrary course.

Tailor examples and pacing to the audience's stated role, topic familiarity, and learning goal. Do not assume expertise in a new subject from experience in another field. Use previous apps as references only when the user requests them; do not embed personal history or identifying details in the skill or generated course.

Capture a compact working brief: topic, audience, starting knowledge, useful end capability, source mode, coverage, and delivery target. Do not demand approval of this brief unless requested. Treat a request to create an app as authorization to build it; follow the platform's publication workflow and existing authorization.

## 2. Ground and organize content

For PDFs, use the available PDF-reading skill. Inspect the contents and extract the requested scope with page/section references. Check figures, tables, code, and OCR where extraction loses meaning. Track coverage so the opening chapters do not accidentally substitute for the whole book. Identify unreadable/missing material; never fill gaps from memory while calling the result document-grounded.

Apply the chosen source mode to **instructional claims, answer keys, distractor explanations, examples, and AI depth**:

| Mode | Content boundary |
| --- | --- |
| Documents only | Derive instructional facts from supplied material. Create original paraphrases and clearly illustrative scenarios using those facts. Do not import outside facts, silent corrections, or unsupported prerequisite teaching. Identify gaps and conflicting passages. Ask to expand the boundary only if an outside prerequisite is essential. |
| Documents + research | Keep the documents as the backbone; research prerequisites, gaps, and current information. Distinguish document claims from additions/updates and cite both. |
| Research assumed | Research before authoring. Prefer authoritative primary sources. Verify changing APIs, service behavior, prices, and certification names/objectives; record the verification date for time-sensitive content. |

Document-only limits concern subject matter, not platform documentation needed to implement the app. Do not label a course current when its only source is an older book. Verify a vaguely named certification rather than substituting a similarly named training course for an exam.

Maintain a source registry and map objectives, cards, and questions to supporting pages/sections or URLs. Expose references through a quiet Sources disclosure. Attribute an author's arguments as arguments; distinguish facts, interpretations, and contested positions. Turn books into original instruction rather than reproducing extensive passages or embedding the whole source by default.

Create a coverage map from source sections to modules/objectives before implementation. Author the requested scope, not placeholders or an outline that appears complete. Organize large topics into short modules and show coverage honestly.

## 3. Teach through recognition and correction

Use **Orient → Recognize → Distinguish → Correct → Re-encounter → Become curious → Ask AI**.

- Give a short orientation about the useful learning outcome. Do not open with a comprehensive system diagram or long reading assignment.
- Identify roughly 5–12 foundational concepts for a broad course, fewer for a narrow one. Introduce names and defining characteristics gradually before expecting complex reasoning.
- Keep one concept and one decision in the main view. Usually present a 50–150-word card, a concrete example, then one MCQ. These are defaults, not reasons to pad or remove necessary meaning.
- Start with easy identification and 2–3 meaningful choices. Progress through distinctions, relationships, scenarios, tradeoffs, and diagnosis, usually with 2–4 choices. Match upper levels to the topic and learner.
- Write plausible distractors from specific misconceptions. Keep alternatives grammatically parallel; avoid joke answers, length clues, trick negatives, and ambiguous keys. Use contrast pairs where adjacent concepts are easily confused.
- Require intentional answer selection/submission. Immediately explain the selected answer and the distinction that matters. Make explanations for other plausible choices available without overwhelming the default view.
- After an error, explain the misconception briefly and allow immediate unlimited retries. Offer hints or a worked explanation when useful. Follow correction with a differently worded question later.
- Revisit each foundational concept in at least three distinct questions across a full course, varying contexts and separating encounters across lessons. If the requested artifact is too short, disclose that limitation instead of padding it. Keep review supportive, without a mandatory flashcard scheduler.
- Use short modules with clear stopping points, usually a few minutes each. Allow review and navigation without punitive locks. Keep free-response exercises and practical labs optional unless the goal calls for them.
- Do not require a giant final exam, unaided recall before every lesson, or a forced holistic overview. Reveal larger relationships once the learner recognizes the components.

Use [learning-design.md](references/learning-design.md) for question/feedback examples and the supporting evidence. Treat exact lengths, recurrence counts, and decorative encouragement as deliberate product choices, not a scientifically proven recipe.

## 4. Encourage every meaningful step honestly

Celebrate a correct answer equally on the first try or after any number of retries. Never qualify success with “finally,” “after three attempts,” a reduced reward, or visible failure counts. Use a compact decorated panel: a checkmark or small sparkle, a soft accent surface, and a message such as **“You got that right!”**, **“That's the distinction.”**, or **“You made the connection.”** Follow it with the useful explanation.

Recognize other progress accurately: “Good move checking the explanation,” “One more concept explored,” or “Welcome back—pick up where you left off.” Use lighter acknowledgment for hints/exploration; reserve correctness language for correct answers. Do not praise an incorrect answer as correct or claim that opening a card proves mastery.

Use warm adult encouragement without infantilizing praise, forced slang, or inflated intelligence claims. No lost lives, streak resets, leaderboards, shame colors, or retry penalties. Corrected answers count toward completion. Keep exposure, completion, and later demonstrated understanding distinct internally; do not equate completion with mastery or guaranteed exam readiness.

Keep feedback visible until the learner continues. Never auto-advance, obstruct reading, or make the learner wait for celebration. Use a restrained one-shot fade/checkmark motion, roughly 150–250 ms, with a static reduced-motion equivalent. No confetti storms, bouncing cards, autoplay sound, or looping decoration.

## 5. Build the working app

Use the requested platform and existing project. For a new hosted app with no other platform preference, use Sites when available: load its building skill, then hosting skill when publishing. Otherwise use the available web-app workflow and state delivery limits honestly. This skill defines learning behavior, not a competing deployment protocol. Complete the functional app rather than stopping at mockups.

- Use modern minimalist typography, generous spacing, restrained borders, neutral surfaces, and a small accent palette. Choose visual details for the topic; avoid a generic dashboard of tiles.
- Build mobile first: single-column lessons, full-width answer targets, readable text, and an obvious Continue action. Expand gracefully on desktop. Aim for touch targets around 44 px, visible focus, semantic controls, and accessible contrast.
- Show concise module progress, a resumable entry point, and an unobtrusive navigator. Put long theory, all-option explanations, and citations in disclosures. Keep essential teaching and selected-answer feedback visible.
- Make states understandable without color. Announce feedback accessibly, manage focus on lesson changes, respect reduced motion, and prevent bottom controls/mobile keyboards from covering content.
- Separate authored course data from presentation. Use stable concept/lesson/question/option IDs, source references, explanations, prerequisites, and curiosity prompts.
- Save progress locally by course ID and content version, including current location and completed question/lesson IDs. Retried success earns completion once; rapid taps/revisits cannot inflate it. Preserve progress on refresh, handle unavailable/corrupt storage gracefully, and make reset deliberate. Do not imply cross-device sync unless implemented.
- Keep content and answer order stable during an attempt. If options shuffle, use IDs for correctness. Never present demo output as commands actually executed on the learner's machine.

End each section with two or three specific, tappable **curiosity prompts** plus an optional custom question. Include the lesson summary and source boundary in the prompt context. With real AI integration, pass that context and enforce the source mode; mark unsupported document-only questions as outside the source. Without integration, provide a working copy/export prompt handoff to the learner's AI, including their custom question, and label it clearly. Never present canned text as a live response or add an API/account requirement merely to finish the core course.

For hands-on topics, supply copyable commands/prompts, expected outcomes, and useful troubleshooting. Distinguish learn, try on your machine, and demo states. Verify runnable examples with available tools when feasible.

## 6. Verify and deliver

Check content and the actual learner path, not just whether the app builds:

- Inspect foundational and later questions for unsupported claims, ambiguity, prerequisite jumps, repeated wording, and source drift. Check coverage and varied encounters in course data.
- Exercise correct-first-try, multiple-wrong-then-correct, hint/reveal, revisit, refresh/resume, completion, and reset. Confirm equal encouragement and completion credited once.
- Inspect a narrow phone viewport and desktop. Check keyboard navigation, visible feedback, reduced motion, overflow, and usable controls.
- Exercise curiosity chips/custom input: verify live contextual AI if present, or actual clipboard/export content for a handoff. Check citation/copy controls.
- Run required builds and targeted checks addressing these risks. Fix discovered failures; identify unverified behavior instead of claiming it passed.

Deliver the working preview or published link, a short description of audience/coverage, the chosen source mode, and material limitations. Avoid a long process report.
