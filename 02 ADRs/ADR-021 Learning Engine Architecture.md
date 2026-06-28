# ADR-021: Learning Engine Architecture

## Status

Accepted

---

# Context

The primary purpose of LEA is not knowledge storage but learning effectiveness.

Existing learning systems largely focus on content management, while LEA aims to engineer the cognitive process of learning itself.

The Learning Engine is therefore responsible for transforming a learner from initial exposure to deep understanding through a structured sequence of learning processes.

Knowledge generated during learning must be transformed into reusable Knowledge Assets and transferred to the Knowledge Engine for refinement and long-term management.

The Knowledge Engine, in turn, continuously feeds curated knowledge back into the Learning Engine, creating a closed-loop learning system.

---

# Decision

Introduce the **Learning Engine** as a core capability responsible for orchestrating the learner's cognitive journey.

The Learning Engine shall consist of a set of reusable learning processes.

### Learning Processes

1. Theme Discovery
2. Theme Exploration
3. Dialectic Learning
4. Multidimensional Reasoning
5. Knowledge Asset Creation

Additional processes such as Reflection, Active Recall, and Spaced Reinforcement may be incorporated in future releases.

---

# Knowledge Asset Creation

Knowledge Asset Creation is the final process of the Learning Engine.

Its responsibility is to convert transient learning outcomes into structured candidate Knowledge Assets.

Typical outputs include:

- Theme updates
- Knowledge Objects
- Theme Maps
- Cross-theme relationships
- Question Envelopes
- Composite Themes
- Learning insights
- Architecture Decisions (when applicable)

Ownership of these assets is then transferred to the Knowledge Engine.

---

# Learning–Knowledge Feedback Loop

The Learning Engine and Knowledge Engine operate as a reinforcing feedback loop.

Learning Engine

↓

Candidate Knowledge Assets

↓

Knowledge Engine

↓

Curated Knowledge Assets

↓

Learning Engine

The Learning Engine never consumes raw discussions as reusable knowledge.

Instead, it consumes curated Knowledge Assets provided by the Knowledge Engine.

---

# Responsibilities

### Learning Engine

- Drive learning conversations
- Facilitate exploration
- Challenge assumptions
- Encourage multidimensional reasoning
- Generate insights
- Produce candidate Knowledge Assets

### Knowledge Engine

- Validate Knowledge Assets
- Organize and classify assets
- Manage Theme relationships
- Eliminate duplication
- Version knowledge
- Feed curated knowledge back into learning

---

# Rationale

This architecture separates learning from knowledge management while enabling continuous improvement through a closed-loop feedback system.

It maintains clear ownership boundaries and supports scalable evolution of both engines.

---

# Consequences

## Positive

- Clear separation of responsibilities
- Continuous learning feedback loop
- Reusable learning processes
- Higher quality Knowledge Assets
- Stronger Theme Maps
- Scalable architecture

## Trade-offs

- Requires explicit handoff between engines
- Introduces governance for candidate vs. curated Knowledge Assets
- Increases coordination between Learning and Knowledge Engines

---

# Future Work

- Reflection Engine
- Active Recall Process
- Spaced Reinforcement Process
- Adaptive reasoning templates
- Learning analytics
- Personalized learning pathways