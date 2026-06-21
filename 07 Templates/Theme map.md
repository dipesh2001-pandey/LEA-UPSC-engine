

# LEA Theme Map Template v1.0

## Purpose

A Theme Map is the conceptual relationship model of a Theme.

It does not store knowledge.

It visualizes how a Theme connects to the rest of the Learning Enterprise Architecture (LEA).

The Theme remains the single source of truth.

The Theme Map is implemented in Obsidian using a **Canvas**.

---

# Deliverables

Every **Composite Theme** shall produce two artifacts:

```
Composite Theme (.md)

+

Theme Map (.canvas)
```

Example:

```
Executive/
│
├── Executive.md
├── Executive.canvas
├── President.md
├── Vice President.md
├── Prime Minister.md
├── Council of Ministers.md
└── Cabinet.md
```

---

# Theme Map Design Principles

- Theme Maps contain **Theme nodes only**.
- Theme Maps never duplicate Theme content.
- Every node represents exactly one Theme.
- Every connection has semantic meaning.
- The Theme should remain the single source of truth.
- The Canvas is the visual implementation of the Theme Map.
- The map should be understandable within 30 seconds.
- Simplicity is preferred over completeness.

---

# Canonical Canvas Layout

```
                 Prerequisite Themes
                         ▲
                         │

                ┌────────────────┐
                │ Current Theme  │
                └────────────────┘

                         │
                         ▼

                Connected Themes

                         │
                         ▼

                  Future Themes
```

---

# Canvas Sections

## 1. Prerequisite Themes

Themes that should ideally be understood before studying the current Theme.

---

## 2. Current Theme

The Composite Theme being modeled.

Acts as the central node of the map.

---

## 3. Connected Themes

Themes directly related to the current Theme.

Examples include:

- Parent Themes
- Child Themes
- Sibling Themes
- Cross-domain Themes
- Frequently Compared Themes

---

## 4. Future Themes

Themes discovered during learning that deserve independent implementation later.

These represent opportunities for future expansion of LEA.

---

# Relationship Types

Every edge should carry semantic meaning.

Suggested relationship types:

- Prerequisite
- Part Of
- Depends On
- Extends
- Contrasts With
- Frequently Compared
- Cross-Domain
- Leads To

---

# Canvas Rules

- Only Theme nodes are permitted.
- Concepts belong inside Themes.
- Facts belong inside Themes.
- Articles belong inside Themes.
- Case laws belong inside Themes.
- Current Affairs belong inside Themes.
- Theme Maps model relationships only.
- Theme Maps complement Themes; they never replace them.

---

# Architecture Principle

> Physical hierarchy exists for storage.

> Logical hierarchy emerges through Theme Maps and interconnected Themes.

The Theme Map is the visual representation of the LEA Knowledge Graph.

---

# Definition of Done

A Theme Map is complete when:

- The Composite Theme is the central node.
- All prerequisite Themes are connected.
- All major related Themes are connected.
- Future Themes have been identified.
- Relationship types are meaningful and consistent.
- The Canvas remains simple, readable, and cognitively efficient.