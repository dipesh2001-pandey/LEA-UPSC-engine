# Design Journal

**Sprint:** Genesis

**Date:** 2026-06-20

---

# Architectural Review

## Topic

Capability Identification

---

# Observation

Early capability discovery produced more than twenty candidate capabilities.

Examples included:

- Revision
- Recall
- Search
- Feedback
- Planning
- Reinforcement
- Error Analysis
- Knowledge Acquisition

While individually meaningful, many represented implementation details or operational activities rather than enduring enterprise capabilities.

The architecture was becoming unnecessarily fragmented.

---

# Realization

Enterprise capabilities should represent **stable business abilities**, not every important activity performed by the system.

Many previously identified capabilities were more appropriately modeled as:

- Capability Areas
- Domain Services
- Processes
- Technical Services

rather than top-level enterprise capabilities.

---

# Decision

The capability model was simplified into four Level 1 capabilities.

## Business

- Knowledge Management
- Learning Management
- Assessment Management

## Governance

- Architecture Governance & Evolution

Detailed responsibilities were preserved as Level 2 capability areas rather than promoted to enterprise capabilities.

---

# Architectural Impact

This decision establishes a stable enterprise backbone from which the remainder of LEA will emerge.

Future architectural work will derive:

- Capability interactions
- Bounded contexts
- Engines
- Stocks
- Flows
- Processes
- Workflows

from these four enterprise capabilities.

---

# Assumptions Invalidated

### Previous Assumption

Every important responsibility should become a top-level capability.

### New Understanding

Only enduring business abilities belong at the enterprise capability level.

Everything else should emerge through decomposition.

---

# New Architecture Principle

> Keep the enterprise capability model intentionally small.

Complexity should emerge only where implementation proves it necessary.

---

# Next Architectural Objective

Design the **Capability Interaction Map**.

This will identify:

- Capability dependencies
- Natural clusters
- Bounded contexts
- Candidate engines

without prematurely fixing implementation boundaries.

---

# Reflection

This session marked the transition from conceptual architecture to enterprise architecture.

Instead of thinking in terms of study activities or tools, LEA now models the learning enterprise through enduring business capabilities.

This significantly increases architectural stability and ensures that future implementation decisions remain capability-driven rather than tool-driven.