# ADR-009: Learning Management Capability

**Status:** Accepted

**Date:** 2026-06-20

---

# Context

Knowledge alone does not produce learning.

A learner may possess high-quality Knowledge Assets yet still fail to understand, retain, apply or recall them effectively.

Knowledge Management governs the enterprise Knowledge Stock.

A separate enterprise capability is required to transform that knowledge into durable learner capability.

---

# Decision

Learning Management is the enterprise capability responsible for governing the learner's cognitive transformation.

It manages the complete learning lifecycle from initial exposure to mastery and continuously improves the learner's Learning State.

Learning Management owns the **Learning State** of LEA.

---

# Purpose

To transform enterprise knowledge into durable understanding, retention, application and mastery for UPSC preparation.

---

# Scope

Learning Management is responsible for:

- Learning Planning
- Knowledge Internalization
- Understanding
- Reinforcement
- Retention
- Recall Readiness
- Mastery Development
- Learning Progress
- Learning Strategy
- Cognitive Load Management

Learning Management is **not** responsible for:

- Knowledge creation
- Knowledge organization
- Assessment
- Performance measurement
- Study resource management

These belong to other enterprise capabilities.

---

# Learning State

Learning Management owns the enterprise Learning State.

The Learning State represents the learner's evolving cognitive relationship with the Knowledge Stock.

Examples include:

- Exposure
- Understanding
- Confidence
- Retention
- Recall Readiness
- Mastery

The exact information model will be defined in a future ADR.

---

# Inputs

Learning Management consumes:

- Knowledge Assets
- Theme Relationships
- Learner Time
- Learning Activities
- Assessment Feedback

---

# Outputs

Learning Management produces:

- Improved Learning State
- Learning Readiness
- Assessment Readiness
- Learning Insights

---

# Architectural Principles

## Learner-Centric

Learning occurs within the learner.

LEA facilitates learning but cannot replace the learner's cognitive effort.

---

## Continuous Learning

Learning is an iterative process.

Every interaction with a Theme may improve the Learning State.

---

## Knowledge-Driven Learning

Learning Management consumes Knowledge Assets but never owns them.

Knowledge ownership remains with Knowledge Management.

---

## Learning Before Assessment

Assessment measures learning but does not replace it.

Learning precedes assessment.

---

## Separation of Concerns

Learning Management owns the learner's cognitive state.

Knowledge Management owns the enterprise Knowledge Stock.

Assessment Management owns performance evaluation.

---

# Collaboration

Learning Management collaborates with:

- Knowledge Management
- Assessment Management
- Architecture Governance & Evolution

Ownership of the Learning State always remains with Learning Management.

---

# Consequences

## Positive

- Clear separation between knowledge and learning.
- Learning becomes an enterprise capability rather than a collection of study techniques.
- Supports multiple learning strategies without changing the architecture.
- Provides a stable foundation for future Learning Engines and processes.

---

## Trade-offs

- The Learning State is intentionally abstract at this stage.
- Detailed learning processes and strategies are deferred until the process-design phase.

---

# Architecture Principle

> **Knowledge informs learning, but only the learner creates learning.**

Learning Management governs the transformation of enterprise knowledge into durable learner capability while preserving the learner as the central actor in the learning process.