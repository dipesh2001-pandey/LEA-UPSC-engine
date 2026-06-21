# ADR-019: ChatGPT Project Architecture for LEA

## Status

Accepted

---

## Context

With the completion of the Knowledge Engine and Learning Engine architecture, LEA requires an operational implementation for dialectic learning.

A decision was needed on how ChatGPT should be integrated into the Learning Engine while preserving the architectural separation between learning and knowledge management.

The implementation should:

- Support bounded contexts.
- Minimize cognitive overhead.
- Prevent cross-domain context contamination.
- Preserve Obsidian as the canonical Knowledge Engine.
- Enable continuous dialectic learning.

---

## Decision

ChatGPT Projects shall function as **Learning Engine bounded contexts**, while Obsidian shall remain the **Knowledge Engine**.

The following project structure is adopted:

```text
LEA Architecture
│
├── LEA Strategy Office
│
├── GS1 Learning Engine
├── GS2 Learning Engine
├── GS3 Learning Engine
├── GS4 + Essay Learning Engine
└── Philosophy Optional Learning Engine
```

### Project Responsibilities

#### LEA Architecture

Responsible for:

- Enterprise Architecture
- ADRs
- Engine Design
- Templates
- Continuous Architectural Evolution

---

#### LEA Strategy Office

Responsible for:

- Subject Analysis
- Syllabus Analysis
- PYQ Analysis
- Resource Selection
- Study Planning
- Sprint Planning
- Learning Strategy
- Enterprise Governance

This project does **not** perform Theme discussions.

---

#### GS Learning Engine Projects

Each GS project functions as a dialectic learning workspace.

Responsibilities include:

- Concept clarification
- Socratic discussions
- Mental model construction
- Cross-theme reasoning
- Theme refinement
- Answer discussion
- Application support

These projects do **not** store canonical knowledge.

---

#### Philosophy Optional Learning Engine

Dedicated bounded context for Philosophy Optional.

Maintains complete separation from General Studies.

---

## Knowledge Ownership

ChatGPT Projects are **temporary learning workspaces**.

Obsidian remains the single source of truth.

Only validated understanding is compiled into Themes.

---

## Learning Workflow

```text
External Source
        │
        ▼
ChatGPT Learning Project
(Dialectic Learning)
        │
        ▼
Knowledge Engine
(Obsidian Themes)
        │
        ▼
Revision
Application
Reflection
```

The Learning Engine and Knowledge Engine operate in a continuous feedback loop during knowledge construction.

---

## Rationale

This architecture provides:

- Clear bounded contexts.
- Separation of learning and knowledge.
- Reduced context contamination.
- Improved continuity of discussions.
- Reusable enterprise design.
- Minimal operational complexity.

---

## Consequences

### Positive

- ChatGPT becomes a dedicated dialectic learning partner.
- Knowledge remains centralized within LEA.
- Discussions naturally evolve into higher-quality Themes.
- Projects remain focused on specific learning domains.
- Architecture remains scalable across subjects and future implementations.

### Trade-offs

- Multiple ChatGPT projects must be maintained.
- Architectural discipline is required to prevent knowledge duplication.

---

## Architecture Principles Established

1. ChatGPT belongs to the Learning Engine.
2. Obsidian belongs to the Knowledge Engine.
3. Learning conversations precede documentation.
4. Themes are compiled from mature understanding.
5. ChatGPT Projects are bounded contexts, not knowledge repositories.
6. Obsidian remains the canonical source of truth.
7. Knowledge construction occurs through a Learning–Knowledge feedback loop.

---

## Future Work

- Design operational workflows for each Learning Engine project.
- Implement Assessment Engine.
- Implement Governance Engine.
- Define AI interaction patterns for dialectic learning.
- Develop learning analytics across projects.