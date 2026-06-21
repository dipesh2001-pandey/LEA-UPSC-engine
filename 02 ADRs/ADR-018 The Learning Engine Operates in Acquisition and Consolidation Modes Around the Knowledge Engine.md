# ADR-018: The Learning Engine Operates in Acquisition and Consolidation Modes Around the Knowledge Engine

## Status

Accepted

---

# Context

During Sprint 2, the Learning Enterprise Architecture (LEA) modeled the enterprise as a sequential flow where the Knowledge Engine produced Themes that were subsequently consumed by the Learning Engine.

During Sprint 3 implementation, this assumption proved incomplete.

Real learning does not begin with knowledge organization. It begins with exposure to external learning sources such as lectures, books, classroom discussions, and current affairs. The learner first develops an initial understanding before organizing it into a structured knowledge model.

Furthermore, learning does not end once a Theme is created. The canonical Theme becomes the foundation for higher-order learning through retrieval practice, revision, interleaving, answer writing, and reflection. These activities generate new cognitive insights that continuously refine the Theme.

Implementation therefore revealed that the Learning Engine exists both before and after the Knowledge Engine.

---

# Decision

The Learning Engine shall operate in two distinct modes.

## 1. Acquisition Mode

Purpose: Transform external learning resources into initial understanding.

Inputs:

- Lectures
- Books
- PDFs
- Current Affairs
- Classroom discussions
- Personal observations

Outputs:

- Raw concepts
- Questions
- Initial understanding
- Candidate relationships

These outputs become the input to the Knowledge Engine.

---

## 2. Consolidation Mode

Purpose: Transform canonical Themes into durable understanding.

Inputs:

- Canonical Theme
- Theme Map

Activities include:

- Retrieval practice
- Revision
- Feynman explanation
- Mental model construction
- Interleaving
- Practice questions
- Answer writing
- Connection building

Outputs:

- Cognitive assets
- Refined understanding
- Improved explanations
- Newly discovered relationships
- Learning insights

These outputs are fed back to the Knowledge Engine for evaluation and incorporation into the canonical Theme.

---

# Enterprise Dynamics

```text
External Sources
        │
        ▼
Learning Engine
(Acquisition)
        │
        ▼
Knowledge Engine
(Cognitive Core)
        │
        ▼
Learning Engine
(Consolidation)
        │
        ▼
Assessment Engine
        │
        ▼
Governance Engine
        │
        └──────────────► Continuous Improvement
```

The Knowledge Engine serves as the Cognitive Core of LEA, while the Learning Engine surrounds it through continuous acquisition and consolidation.

---

# Rationale

This decision more accurately reflects how humans learn.

Knowledge is first experienced, then organized, then repeatedly reinforced.

Separating the Learning Engine into Acquisition and Consolidation modes preserves clear ownership boundaries while enabling continuous feedback into the canonical knowledge model.

The Theme becomes the shared enterprise artifact exchanged between engines throughout the learning lifecycle.

---

# Consequences

## Positive

- Aligns LEA with natural human learning processes.
- Establishes a closed feedback loop between learning and knowledge organization.
- Reinforces the Theme as the canonical knowledge artifact.
- Clarifies engine responsibilities without introducing additional engines.
- Supports continuous refinement of Themes through implementation feedback.

## Trade-offs

- The Learning Engine is no longer modeled as a purely downstream consumer.
- Enterprise dynamics become cyclical rather than strictly sequential.
- Theme refinement becomes an ongoing capability instead of a one-time activity.

---

# Architecture Principle

> The Learning Engine acquires knowledge before the Theme exists and consolidates knowledge after the Theme is created. The Knowledge Engine continuously transforms these learning experiences into an increasingly accurate canonical representation of the domain.

---

# Future Work

- Define the operational workflow for Acquisition Mode.
- Design the standard Theme Template consumed by both Learning Engine modes.
- Define how learning insights are validated before incorporation into the canonical Theme.
- Operationalize the Theme Map as the structural representation of conceptual relationships.