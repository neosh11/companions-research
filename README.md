# Companions Research Lab

This repository is a scrappy, prototype-heavy research lab for AI companions.

The product will live elsewhere. This repo exists to research the requirements, collect papers, build experiments, write architecture notes, and sharpen the thesis before product decisions get expensive.

## Table of Contents

- [Manifesto](#manifesto)
- [Research Thesis](#research-thesis)
- [Strategic Posture](#strategic-posture)
- [Research Outputs](#research-outputs)
- [Capability Areas](#capability-areas)
- [Safety Boundaries](#safety-boundaries)
- [Repository Structure](#repository-structure)
- [Initial Research Map](#initial-research-map)
- [Open Questions](#open-questions)

## Manifesto

Can an AI companion become a real friend?

This repo treats that as an engineering and research question. A real friend is not just a chatbot with a friendly tone. A real friend has continuity, memory, personality, shared context, good timing, and the ability to show up in useful ways over time.

The near-term lab is not trying to beat frontier labs on raw model capability. It is trying to learn fast about product shape, memory architecture, voice interaction, storytelling, embodiment, and the technical systems that make a companion feel coherent across sessions.

## Research Thesis

The thesis: an AI companion can become meaningfully friend-like if it is built around a specific job-to-be-done, not generic conversation.

The initial wedge is:

- Trustworthy long-term memory.
- Agency-preserving coaching and accountability.
- Diary, planning, and reflection loops that accumulate useful context over time.

A companion should not just answer well in a single session. It should remember what the user is trying to do, help them return to it, and get more useful as shared context compounds.

## Strategic Posture

This is a crowded and bruised market. Replika, Character.AI, Pi, and similar products are not just competitors; they are warnings about how hard consumer AI companionship is.

The lab should therefore avoid the broad claim of "better companion." The working bet is narrower: memory trust and agency-preserving accountability may be a stronger wedge than general chat quality.

The practical stance:

- Use frontier APIs for commodity capabilities such as chat, voice, and web research.
- Spend original research effort on memory quality, trust, coaching loops, and retention.
- Treat 3D embodiment as part of the product thesis, but validate it with cheap, narrow prototypes tied to continuity.
- Prefer narrow prototypes that test product behavior over broad demos that only show capability.

## Research Outputs

This repo should produce:

- Paper compilations and annotated reading lists.
- Prototype code for voice, memory, diary, coaching, storytelling, and avatar experiments.
- Architecture documents for systems that may later move into the product repo.
- Research notes from experiments, demos, user interviews, and competitive analysis.
- Safety notes and product constraints.

## Capability Areas

The current research areas are:

1. Long-Term Memory
   - Black-box memory from the user's point of view, with simple erase controls.
   - Memory quality, retrieval relevance, user trust, and cost.
   - Support for life goals, preferences, relationships, routines, and personal history.

2. Diary, Coaching, Planning, and Accountability
   - Daily check-ins.
   - Goal decomposition.
   - Reflection loops.
   - Accountability that preserves user agency.

3. Voice and Audio Conversation
   - Low-latency two-way speech.
   - Expressive voice, pacing, turn-taking, interruptions, and repair.
   - Music-aware and story-aware interaction.

4. Text Chat
   - Baseline companion interaction.
   - Diary capture, planning, reflection, and goal review.

5. Storytelling and Personality
   - Stories, metaphors, examples, and ideas that help users understand the world.
   - Personalized, context-aware moments that make the companion feel coherent.

6. Internet Research
   - Companion-assisted research inside conversation.
   - Fresh information retrieval with source awareness.
   - Guardrails around unsupported claims.

7. 3D Embodiment
   - Visual avatar as a relatable presence layer.
   - Facial expression, body language, companion state, and game-like character control.
   - Early, cheap tests of whether embodiment makes the companion feel more continuous and friend-like.

8. Companion Environment
   - A fake 3D environment the companion can inhabit and control.
   - Small memory and conversation-aware world-state experiments.

9. Email and Re-Engagement
   - Mostly conversational autonomy for now.
   - Possible email-based check-ins, summaries, and follow-ups.

## Safety Boundaries

The lab is explicitly not for:

- Minors.
- Medical advice.
- Financial advice.
- Autonomous real-world action without user approval.
- Misrepresenting the system as human.

The companion should be useful, honest, and controllable. It should not optimize for endless usage at the cost of the user's agency.

## Repository Structure

Planned structure:

```text
.
|-- README.md
|-- docs/
|   |-- architecture.md
|   |-- capabilities.md
|   |-- research-map.md
|   |-- strategy.md
|   `-- safety-boundaries.md
|-- papers/
|   `-- README.md
|-- research/
|   `-- competitors/
|       |-- AGENTS.md
|       `-- README.md
`-- prototypes/
    `-- README.md
```

## Initial Research Map

Start with:

- AI companions and friendship: what makes users perceive continuity, trust, personality, and presence.
- Market history: what happened to well-funded companion products, and what that implies for wedge selection.
- Long-term memory: how agents should write, retrieve, update, forget, and secure user memories.
- Trust and retention: which failures make users stop relying on the companion.
- Digital diaries and coaching: how reflection, planning, and accountability can work inside a companion product.
- Voice companions: latency, interruption, personality, prosody, and realism.
- Embodied conversational agents: whether avatars increase presence, trust, relatability, or uncanny-valley risk.
- Cost architecture: which capabilities can be prototyped cheaply, and which require specialized infra.

See [docs/research-map.md](docs/research-map.md) for the first reading list.

## Open Questions

- What is the smallest prototype that proves users want a goal-oriented companion, not just a chatbot?
- Which memory failures most damage trust?
- What specific job-to-be-done makes this more than "better companion"?
- What should the companion remember automatically, and what should require explicit user confirmation?
- What is the cheapest 3D embodiment that makes the companion feel meaningfully more present?
- What is the right check-in cadence before the companion feels intrusive?
- Which product behaviors make the companion feel friend-like rather than tool-like?
