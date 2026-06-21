# ADR-020: Engines are Defined by Their Primary Stock

**Status:** Accepted

---

# Context

During the design of the Governance Engine, a fundamental systems thinking question emerged:

> _What fundamentally distinguishes one Engine from another?_

Previous ADRs established that an Engine represents a bounded business domain with its own purpose, capabilities, information model, artifacts, and lifecycle. However, the architecture lacked a systems-thinking principle explaining **what each Engine is ultimately responsible for managing**.

Without this distinction, Engine boundaries risk becoming capability-driven rather than purpose-driven, resulting in overlapping responsibilities and unclear ownership.

---

# Decision

Every Engine shall be defined by **one Primary Stock**.

A **Primary Stock** is the enterprise asset that an Engine is responsible for creating, maintaining, protecting, and improving over time.

Capabilities, processes, workflows, and implementations exist solely to manage the Engine's Primary Stock.

The LEA Enterprise consists of four Engines, each stewarding a unique enterprise asset.

|Engine|Primary Stock|Enterprise Asset|
|---|---|---|
|Learning Engine|Learner Competence|Human Capital|
|Knowledge Engine|Canonical Knowledge|Intellectual Capital|
|Assessment Engine|Assessment Evidence|Evidence Capital|
|Governance Engine|Enterprise Intelligence|Strategic Capital|

---

# Rationale

This decision unifies **Systems Thinking** with **Enterprise Architecture**.

Each Engine now possesses:

- A unique enterprise purpose.
- A unique stock under its stewardship.
- Clear ownership boundaries.
- Independent evolution.
- Explicit information exchanges with other Engines.

An Engine is therefore distinguished not by the activities it performs, but by the **enterprise asset it owns and continuously improves**.

---

# Engine Responsibilities

## Learning Engine

**Primary Stock:** Learner Competence

Responsible for transforming the learner through understanding, internalization, integration, reinforcement, application, and reflection.

---

## Knowledge Engine

**Primary Stock:** Canonical Knowledge

Responsible for creating, organizing, validating, publishing, and evolving Themes, Theme Maps, and other knowledge assets.

---

## Assessment Engine

**Primary Stock:** Assessment Evidence

Responsible for objectively measuring learning and generating evidence regarding competency, progress, strengths, and weaknesses.

---

## Governance Engine

**Primary Stock:** Enterprise Intelligence

Responsible for continuously improving the Learning Enterprise through strategy, standards, architecture governance, performance management, and evidence-based decision-making.

Governance governs the enterprise but does **not** own the operational stocks managed by the Learning, Knowledge, or Assessment Engines.

---

# Enterprise Feedback Model

```text
                    Governance Engine
                 Enterprise Intelligence
                          ▲
                          │
        ┌─────────────────┼─────────────────┐
        │                 │                 │
        │                 │                 │
Assessment          Knowledge         Learning
 Evidence           Knowledge         Competence
```

Information flows upward into Governance.

Governance produces decisions, standards, policies, and improvement initiatives that guide the operational Engines.

---

# Consequences

## Positive

- Establishes a systems-thinking foundation for LEA.
- Clearly differentiates Engines from Capabilities.
- Prevents overlapping ownership.
- Strengthens bounded contexts.
- Supports independent evolution of each Engine.
- Enables enterprise-wide optimization through feedback loops.

## Trade-offs

- Every future Engine proposal must identify a unique Primary Stock before being accepted.
- Architectural discipline must be maintained to avoid capability duplication across Engines.

---

# Architecture Principle

> **An Engine is defined by the enterprise asset (Primary Stock) it stewards. Capabilities, processes, workflows, and implementations exist solely to create, maintain, improve, and govern that stock.**

---

# Future Work

- Define the inflows and outflows for each Primary Stock.
- Design stock-level KPIs for every Engine.
- Model reinforcing and balancing feedback loops across the enterprise.
- Use Primary Stocks as the basis for Governance dashboards and enterprise health monitoring.

---

# Related ADRs

- ADR-001 – LEA Vision and Purpose
- ADR-002 – Theme as the Atomic Knowledge Unit
- ADR-008 – Four Engine Enterprise Architecture
- ADR-009 – Capability-Driven Engine Design