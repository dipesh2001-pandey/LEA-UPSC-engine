# ADR-015: Enterprise Engine Architecture

**Status:** Accepted

**Sprint:** Sprint 2 – Enterprise Dynamics

---

# Context

Sprint 1 established the static architecture of LEA through Enterprise Capabilities and Enterprise Stocks.

While Capabilities define ownership, they do not describe enterprise behaviour or value transformation.

Sprint 2 introduced Enterprise Engines to model the dynamic behaviour of the Learning Enterprise.

---

# Decision

LEA shall model enterprise behaviour using four Enterprise Engines.

- Knowledge Engineering Engine
- Learning Engine
- Assessment Engine
- Governance & Evolution Engine

Each Engine is responsible for transforming one enterprise state into another while interacting with other Engines through well-defined contracts, enterprise events and feedback loops.

---

# Architecture

```text
Enterprise Capability
        │
        ▼
Enterprise Engine
        │
        ▼
Pipeline
        │
        ▼
Processes
        │
        ▼
Workflows
```

---

# Principles

- Capabilities own enterprise stocks.
- Engines transform enterprise stocks.
- Pipelines define engine behaviour.
- Processes implement pipeline stages.
- Workflows orchestrate process execution.

---

# Benefits

- Clear separation between ownership and behaviour.
- Independent Engine evolution.
- Reduced coupling.
- Supports adaptive enterprise design.

---

# Consequences

Future architectural work shall occur primarily within Enterprise Engines while preserving stable Capability boundaries.

---

# Related ADRs

- ADR-012 — Enterprise Engine Layer
- ADR-013 — Canonical Enterprise Engine Meta-Model
- ADR-014 — Information as the Primary Inflow