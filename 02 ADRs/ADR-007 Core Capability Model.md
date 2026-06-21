# ADR-007: Core Capability Model

**Status:** Accepted

**Date:** 2026-06-20

---

# Context

LEA is being designed as a reusable Learning Enterprise Architecture rather than a UPSC-specific study system.

During capability discovery, numerous candidate capabilities were identified, including Knowledge Acquisition, Revision, Recall, Search, Feedback, Error Analysis, Planning, and others.

Architectural review revealed that many of these represented implementation details, processes, or sub-capabilities rather than enduring enterprise capabilities.

To maintain architectural simplicity and support future evolution, a stable enterprise capability model was required before identifying bounded contexts, engines, processes, or workflows.

---

# Decision

LEA adopts a hierarchical capability model.

## Level 1 — Enterprise Capabilities

### Business Capabilities

- Knowledge Management
- Learning Management
- Assessment Management

### Governance Capability

- Architecture Governance & Evolution

These four capabilities represent the highest-level business abilities of the Learning Enterprise Architecture.

---

## Level 2 — Capability Areas

### Knowledge Management

- Knowledge Acquisition
- Knowledge Organization
- Knowledge Relationship Management
- Knowledge Retrieval
- Knowledge Evolution

---

### Learning Management

- Learning Planning
- Learning Execution
- Knowledge Reinforcement
- Recall Management
- Mastery Tracking

---

### Assessment Management

- Assessment Design
- Assessment Execution
- Performance Analysis
- Error Analysis
- Feedback Generation

---

## Out of Scope

The following are intentionally **not** modeled as enterprise capabilities:

- Processes
- Workflows
- Engines
- Technical Services
    - Search
    - Analytics
    - Versioning
    - Synchronization
    - Automation

These will be derived later from the capability model.

---

# Rationale

The adopted model provides:

- A stable enterprise architecture independent of UPSC.
- Clear separation between business capabilities and governance.
- Reduced architectural complexity.
- A foundation for bounded contexts.
- A foundation for engine discovery.
- A capability-first design consistent with Enterprise Architecture and Domain-Driven Design.

The model intentionally favors simplicity at Level 1 while allowing implementation-driven evolution at Level 2.

---

# Consequences

## Positive

- Clear enterprise backbone.
- Easier reasoning about ownership and responsibilities.
- Supports future learning domains beyond UPSC.
- Prevents premature implementation decisions.

## Trade-offs

- Level 2 capability areas may evolve as implementation provides feedback.
- Engine boundaries remain intentionally undecided until capability interactions are modeled.

---

# Future Work

The next architectural activities are:

1. Capability Interaction Mapping
2. Bounded Context Identification
3. Engine Discovery
4. Stock–Flow–Feedback Modeling
5. Information Model Design

---

# Architecture Principle

> Enterprise capabilities represent enduring business abilities.

Processes, workflows, engines, and tools are derived from capabilities—not the other way around.