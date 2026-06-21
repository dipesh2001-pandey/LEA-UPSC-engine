# ADR-008: Knowledge Management Capability

**Status:** Accepted  
**Date:** 2026-06-20

---

# Context

Knowledge is the primary enterprise asset within LEA.

Traditional note-taking systems optimize for storing information, while Knowledge Management Systems primarily optimize retrieval.

LEA has a different objective.

Its purpose is to maximize learning effectiveness for UPSC by enabling the learner to construct, organize, connect and continuously evolve knowledge around syllabus-driven Themes.

The learner is an active participant in the system—not merely a consumer of information.

Knowledge is therefore viewed as a continuously evolving cognitive asset rather than a static collection of notes.

---

# Decision

Knowledge Management is the enterprise capability responsible for governing the complete lifecycle of learner-constructed knowledge.

It ensures that knowledge entering the system matures into high-quality, interconnected Knowledge Assets organized around Themes and continuously evolves through learning, assessment and experience.

Knowledge Management owns the **Knowledge Stock** of LEA.

---

# Purpose

To enable the learner to transform raw knowledge from multiple sources into interconnected, continuously evolving Theme-centric Knowledge Assets optimized for UPSC preparation.

---

# Scope

Knowledge Management is responsible for:

- Knowledge Acquisition
- Knowledge Organization
- Knowledge Classification
- Knowledge Synthesis
- Knowledge Evolution
- Knowledge Retrieval
- Knowledge Relationship Management
- Knowledge Quality & Governance

Knowledge Management is **not** responsible for:

- Learning
- Revision
- Assessment
- Scheduling
- Study Planning
- Learner Performance

These belong to other enterprise capabilities.

---

# Knowledge Lifecycle

```text
Knowledge Source
        ↓
Knowledge Acquisition
        ↓
Transient Knowledge
(Fleeting Notes + Working Notes)
        ↓
Learner Synthesis
        ↓
Theme Assignment
        ↓
Knowledge Asset
        ↓
Knowledge Evolution
        ↓
Living Knowledge Asset
```

Knowledge Assets are never considered complete.

They continuously evolve throughout the learner's preparation.

---

# Knowledge Sources

Knowledge may enter LEA through multiple trusted sources.

## Static Sources

- NCERT
- Standard Reference Books
- Coaching Material
- Constitution
- Government Reports

## Dynamic Sources

- Newspapers
- PIB
- Yojana
- Kurukshetra
- Economic Survey
- Budget
- Government Publications

## Assessment Sources

- PYQs
- Mock Tests
- Mentor Feedback
- Self Review

## Learner Generated Sources

- Personal Insights
- Cross-domain Connections
- Analogies
- Examples
- Theme Refinements

## AI Assisted Sources

- AI Discussions
- AI Explanations
- AI Comparative Analysis
- AI Challenge Sessions

---

# Knowledge Stock

Knowledge Management owns the enterprise Knowledge Stock.

The Knowledge Stock consists of:

- Themes
- Knowledge Assets
- Relationships
- Supporting Metadata

Theme Maps are considered **projections** of the Knowledge Stock rather than independent entities.

---

# Theme

A Theme is the primary knowledge aggregate within LEA.

A Theme represents the smallest learner-owned, cognitively coherent unit of UPSC knowledge that can be independently understood, revised, assessed and connected to other Themes.

Themes provide the organizational boundary within which knowledge evolves.

---

# Knowledge Assets

Knowledge Assets are reusable, high-quality knowledge artifacts owned by a Theme.

Examples include:

- Concept Notes
- Summary Sheets
- Flowcharts
- Timelines
- Comparison Tables
- Diagrams
- Case Compilations
- PYQ Analysis
- Current Affairs Integration
- Revision Sheets

Knowledge Assets continuously evolve throughout preparation.

---

# Architectural Principles

## Learner-Centric Construction

Knowledge is constructed by the learner.

LEA supports construction but never replaces it.

---

## Theme-Centric Organization

Enterprise knowledge is organized around Themes rather than files or folders.

---

## Continuous Evolution

Knowledge Assets are living assets.

Every revision, assessment, discussion or new information may improve an existing asset.

---

## Cognitive Coherence

Themes optimize human understanding rather than database normalization.

Intentional duplication is acceptable when it improves learning effectiveness.

---

## Traceability

Every Knowledge Asset should remain traceable to one or more Knowledge Sources.

---

## Enterprise Knowledge Boundary

Knowledge may exist temporarily outside a Theme during acquisition and synthesis.

However, **no Knowledge Asset becomes part of the enterprise Knowledge Stock until it is intentionally assigned to a Theme by the learner.**

The learner is the gatekeeper of enterprise knowledge.

---

# Collaboration

Knowledge Management collaborates with:

- Learning Management
- Assessment Management
- Architecture Governance & Evolution

Knowledge ownership always remains with Knowledge Management.

---

# Consequences

## Positive

- Theme becomes the stable aggregate for UPSC knowledge.
- Knowledge remains learner-owned.
- Multiple sources contribute to a single evolving Theme.
- Continuous improvement is built into the architecture.
- Knowledge is optimized for learning rather than storage.
- Enterprise Knowledge remains governed while allowing exploratory thinking through Transient Knowledge.

---

## Trade-offs

- Learner synthesis requires greater effort than traditional note-taking.
- Knowledge construction is intentionally slower but produces higher-quality, interconnected Knowledge Assets.
- Theme assignment requires conscious architectural decisions by the learner.

---

# Architecture Principle

> **Knowledge is not collected. It is constructed.**

The learner is the architect of knowledge.

LEA provides the enterprise architecture that enables, governs and continuously evolves that construction.