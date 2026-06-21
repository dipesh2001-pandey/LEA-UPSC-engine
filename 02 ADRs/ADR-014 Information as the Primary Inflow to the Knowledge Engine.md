# ADR-014: Information as the Primary Inflow to the Knowledge Engine

**Status:** Accepted

**Sprint:** Sprint 2 – Enterprise Dynamics

---

# Context

During the design of the Knowledge Engine, an important architectural question emerged:

> **What is the primary unit that flows through the Knowledge Engine?**

Initially, Knowledge Assets appeared to be both the input and output of the Engine.

However, this violates the transformation principle of an Enterprise Engine.

An Engine must transform one state into another.

Therefore, Knowledge Assets cannot simultaneously be the primary input and output.

This review also revealed that LEA is not an isolated enterprise.

It continuously interacts with the **Human Learning System**, which serves as the primary producer and consumer of knowledge.

---

# Decision

The Knowledge Engine shall accept **Information** as its primary inflow.

Information is transformed into **Knowledge Assets**, which are then organized within **Themes** and accumulated in the **Knowledge Stock**.

Knowledge Assets are therefore an **output** of the Knowledge Engine, not its primary input.

---

# Architecture Principle

> **The Knowledge Engine transforms Information into reusable Knowledge Assets organized within Themes, thereby continuously enriching the Enterprise Knowledge Stock.**

---

# Enterprise Context

LEA consists of two interacting adaptive systems.

```text
Human Learning System
        │
        │ Information
        ▼
Knowledge Engine
        │
        │ Knowledge Assets
        ▼
Knowledge Stock
        │
        │ Organized Knowledge
        ▼
Human Learning System
```

The Human Learning System and LEA continuously co-evolve through reinforcing feedback loops.

---

# Information Lifecycle

```text
Information
        │
Acquire
        │
Analyze
        │
Extract
        │
Structure
        │
Create Knowledge Asset
        │
Associate with Theme
        │
Store in Knowledge Stock
```

This transformation defines the core purpose of the Knowledge Engine.

---

# New Domain Object

## Information Input

### Definition

An **Information Input** is any raw information entering the Knowledge Engine that has not yet been transformed into a Knowledge Asset.

Examples include:

- Newspaper articles
- Government reports
- Books
- Coaching lectures
- Videos
- Research papers
- UPSC Previous Year Questions
- Personal observations
- Insights generated during revision
- Discussions and conversations

Information Inputs are transient transformation objects.

Once transformed, they become persistent Knowledge Assets.

---

# Relationship Model

```text
Information Input
        │
        ▼
Knowledge Asset
        │
belongs to
        ▼
Theme
        │
contributes to
        ▼
Knowledge Stock
```

---

# Responsibilities of the Knowledge Engine

The Knowledge Engine shall:

- Acquire Information Inputs
- Validate information quality
- Extract meaningful knowledge
- Structure knowledge
- Create Knowledge Assets
- Associate assets with Themes
- Build relationships between Themes
- Version Knowledge Assets
- Continuously improve the Knowledge Stock

---

# Human Interaction Model

The Human Learning System provides continuous inflows to LEA through:

- Reading
- Observation
- Reflection
- Questioning
- Discussion
- Practice

The Knowledge Engine returns value through:

- Organized knowledge
- Theme discovery
- Knowledge relationships
- Knowledge gap identification
- Structured retrieval
- Recommendations for further learning

This creates a reinforcing feedback loop that improves both the learner and the enterprise.

---

# Benefits

This decision:

- Clearly separates inputs from outputs.
- Preserves the transformation semantics of an Enterprise Engine.
- Establishes a clean interface between the Human Learning System and LEA.
- Provides a foundation for continuous knowledge acquisition.
- Supports multiple future information sources without architectural change.

---

# Consequences

The Knowledge Engine will no longer be modeled as a repository.

Instead, it will be modeled as a **continuous transformation system**.

Future process design will focus on transforming Information Inputs into high-quality Knowledge Assets.

Other Engines will consume Knowledge Assets from the Knowledge Stock rather than raw Information Inputs.

---

# Related ADRs

- ADR-008 — Enterprise Capability Model
- ADR-009 — Enterprise Stock Ownership
- ADR-011 — Enterprise Capability Layer
- ADR-012 — Enterprise Engine Layer
- ADR-013 — Canonical Enterprise Engine Meta-Model

---

# Design Journal

## Observation

Knowledge Assets cannot simultaneously be both the input and output of the Knowledge Engine.

The true inflow originates from the Human Learning System in the form of raw Information.

---

## Decision

Introduce **Information Input** as the primary inflow to the Knowledge Engine.

The Engine transforms Information into reusable Knowledge Assets organized within Themes.

---

## Why It Changed

Applying systems thinking revealed that LEA and the Human Learning System form a coupled adaptive system.

This required distinguishing between transient Information and persistent Knowledge.

---

## Consequence

The Knowledge Engine is now defined as a **knowledge transformation engine**, not merely a knowledge repository.

This establishes the first explicit interaction model between the learner and the Learning Enterprise Architecture and provides the foundation for all subsequent engine design.