# Architecture Notes

The product architecture will live elsewhere. This repo keeps experimental architecture notes and prototype findings.

## Working System Shape

```text
User
  -> voice or text interface
  -> conversation orchestrator
  -> memory layer
  -> planning and diary tools
  -> research tools
  -> story and coaching policies
  -> voice output
  -> avatar and optional environment controller
```

## Core Components

### Conversation Orchestrator

Owns turn-taking, tool use, persona consistency, product boundaries, and routing between chat, diary, coaching, storytelling, research, and avatar control.

### Memory Layer

The user experience can be black-box, but the implementation needs clear internal structure:

- Raw conversation history.
- Diary entries.
- User facts and preferences.
- Goals, plans, and accountability state.
- Important relationships.
- Recurring themes.
- User-visible erase controls.

### Diary and Coaching Layer

Turns conversation into:

- Reflections.
- Goals.
- Next actions.
- Plans.
- Follow-up prompts.
- Accountability summaries.

### Storytelling Layer

Generates stories, ideas, metaphors, and examples grounded in user context without pretending to have human experience.

### Voice Layer

Research questions:

- How low must latency be before the companion feels responsive?
- Which interruptions should be supported?
- How much prosody and expressiveness can be added cheaply?
- Which voice failures break trust?

### Avatar Layer

The avatar should express attention, personality, and conversational state. The first version should be constrained and cheap: enough to test presence and continuity, not enough to become a full graphics pipeline.

## Cost Questions

- Which memory operations need expensive model calls?
- Which summaries can run asynchronously?
- How small can the voice stack be while still feeling present?
- What is the cheapest avatar pipeline that still feels expressive?
- Which features can be mocked before infra is built?
