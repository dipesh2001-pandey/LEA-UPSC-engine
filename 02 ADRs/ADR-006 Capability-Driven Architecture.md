
ADR-006: Capability-Driven Architecture

| Status | Accepted |
|---------|----------|
| Date | 2026-06-20 |
| Version | LEA v0.1 |
| Category | Core Architecture |

---

# Context

As the Learning Enterprise Architecture (LEA) evolved, the architecture began accumulating several "engines" such as:

- Learning Engine
- Revision Engine
- Current Affairs Engine
- Practice Engine
- Analytics Engine

During the architecture review it became evident that these represented a mixture of **capabilities**, **processes**, and **implementations**.

This violated one of the fundamental principles of systems thinking:

> Every subsystem should exist only if it owns a unique responsibility, state and feedback loop.

The architecture required a higher level of abstraction.

---

# Decision

LEA shall be designed around **Capabilities** rather than features, tools, workflows or implementation details.

Capabilities represent **what the system must be able to do**, independent of how those capabilities are implemented.

Every future architectural component must support one or more capabilities.

Capabilities become the primary architectural building blocks of LEA.

---

# Rationale

Capabilities are:

- Stable
- Technology independent
- Long-lived
- Outcome-oriented
- Implementation agnostic

Unlike tools or workflows, capabilities rarely change even when implementations evolve.

For example:

Capability

↓

Build Knowledge

can be implemented using

- Obsidian
- Paper Notes
- AI Assistant
- Future Technologies

The capability remains unchanged.

---

# Capability Hierarchy

```
Capability

↓

Engine

↓

Process

↓

Workflow

↓

Implementation
```

This hierarchy shall govern all future architectural decisions.

---

# Core Capabilities of LEA

## Knowledge Domain

### Capture Knowledge

Transform external information into structured internal understanding.

---

### Build Knowledge

Transform understanding into reusable Knowledge Assets.

---

### Connect Knowledge

Create relationships between Themes.

Produce Theme Maps and the Knowledge Graph.

---

### Evolve Knowledge

Continuously improve Knowledge Assets through feedback and new learning.

---

## Performance Domain

### Retrieve Knowledge

Recall the right knowledge at the right time.

---

### Apply Knowledge

Transform knowledge into examination performance.

Includes:

- Prelims
- Mains
- Essay
- Interview

---

### Evaluate Knowledge

Measure learning effectiveness through feedback.

Sources include:

- PYQs
- Mock Tests
- Recall Sessions
- Answer Evaluation

---

## Governance Domain

### Govern Learning

Maintain strategic alignment of the learning system.

Responsibilities include:

- Goal Setting
- Prioritization
- Roadmap
- Bottleneck Identification
- Continuous Improvement

---

# Architectural Consequences

This decision establishes the following hierarchy.

```
Vision

↓

Capability Model

↓

Engines

↓

Processes

↓

Workflows

↓

Templates

↓

Tools

↓

Technology
```

Every lower layer must derive from the layer above.

---

# Capability Test

A new capability may only be introduced if it satisfies all of the following conditions.

### Purpose

It has a unique responsibility.

---

### Independence

It can exist independently of implementation.

---

### Outcome

It produces measurable value.

---

### Stability

It is expected to remain valid despite future technology changes.

---

### Longevity

It represents a long-term function rather than a temporary activity.

---

If any condition fails, the proposal should instead be modeled as:

- Process
- Workflow
- Tool
- Implementation

rather than a Capability.

---

# Design Principles

Capabilities define **what** LEA must achieve.

Processes define **how** LEA achieves it.

Tools define **where** LEA is implemented.

Technology defines **with what** LEA is implemented.

---

# Implications

This decision simplifies the architecture by preventing unnecessary proliferation of engines.

For example:

Revision is no longer modeled as an Engine.

Instead,

Revision becomes a Process supporting the Retrieve Knowledge capability.

Similarly,

Current Affairs Integration becomes a Process supporting the Evolve Knowledge capability.

This significantly reduces architectural complexity.

---

# Future Work

The Capability Model will become the central architectural artifact of LEA.

Future work includes:

- Capability Relationships
- Capability Maturity Model
- Capability Ownership
- Capability Metrics
- Capability Dependencies

---

# Guiding Principle

> Design capabilities first.
>
> Everything else is an implementation detail.