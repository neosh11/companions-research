# Strategy

This lab is not trying to win by building a better general-purpose chatbot. The research question is whether an AI companion can become meaningfully friend-like by doing a narrower job better over time.

## Market Caution

Consumer AI companionship has already consumed serious capital and attention.

- [Microsoft announced](https://blogs.microsoft.com/blog/2024/03/19/mustafa-suleyman-deepmind-and-inflection-co-founder-joins-microsoft-to-lead-copilot/) in March 2024 that Inflection co-founders Mustafa Suleyman and Karen Simonyan were joining Microsoft to form Microsoft AI.
- [Character.AI signed](https://www.inc.com/reuters/characterai-signs-licensing-deal-with-google.html) a non-exclusive licensing agreement with Google in August 2024, with co-founders Noam Shazeer and Daniel De Freitas joining Google.

These are not proof that AI companions cannot work. They are evidence that broad consumer companion products are hard, expensive, and strategically fragile.

## Wedge

The wedge cannot be "better companion." It needs to be a specific job-to-be-done.

Working wedge:

- Remember what the user is trying to do.
- Help the user turn diary entries into plans.
- Bring the user back to those plans over time.
- Build enough continuity that the system earns trust across sessions.

## Original Research Effort

Spend research energy on:

- Memory quality.
- Memory explainability and deletion.
- Trust recovery after memory failures.
- Coaching and accountability loops.
- Retention driven by usefulness, not novelty.

Use existing APIs or off-the-shelf systems for:

- General chat quality.
- Speech-to-text.
- Text-to-speech.
- Web retrieval.
- Baseline avatar rendering.

## 3D Posture

3D embodiment is a high-conviction product bet and a real cost risk.

The reason to take it seriously: friendship is not only text. Presence, attention, gesture, shared space, and visible state may be part of what makes a companion feel like a persistent character rather than a chat surface.

The reason to stay disciplined: 3D can absorb huge amounts of time before the core loop works.

Near-term rule:

- Start 3D early, but keep it cheap.
- Test avatar presence as part of continuity, not as a standalone graphics project.
- Avoid custom 3D pipelines until simple embodiment proves it changes user perception.
- Prefer a constrained avatar with expressive state over a broad, customizable world.

## Product-Deciding Questions

- Which memory failures make users stop trusting the companion?
- What makes a proactive check-in useful rather than intrusive?
- What job does the user repeatedly hire the companion to do?
- Does accountability create repeated use without feeling like task management software?
- When does the companion feel friend-like rather than tool-like?
- What does 3D embodiment add that voice and memory cannot?
