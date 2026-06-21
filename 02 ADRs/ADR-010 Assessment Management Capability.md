# ADR-010: Assessment Management Capability

**Status:** Accepted

**Date:** 2026-06-20

---

# Context

Learning without assessment cannot validate progress.

Assessment provides objective evidence of the learner's current capability and generates feedback for both Learning Management and Knowledge Management.

Assessment is not merely a scoring mechanism; it is a continuous feedback capability within LEA.

---

# Decision

Assessment Management is the enterprise capability responsible for evaluating learner performance, identifying learning gaps, and generating actionable feedback to improve both the Learning State and the Knowledge Stock.

Assessment Management owns the **Performance State** of LEA.

---

# Purpose

To continuously measure, validate and improve learner performance throughout UPSC preparation.

---

# Scope

Assessment Management is responsible for:

- Assessment Planning
- Assessment Execution
- Performance Evaluation
- Error Identification
- Feedback Generation
- Readiness Evaluation
- Performance Analytics

Assessment Management is **not** responsible for:

- Knowledge Creation
- Learning
- Revision
- Knowledge Organization
- Study Planning

---

# Performance State

Assessment Management owns the enterprise Performance State.

The Performance State represents measurable evidence of learner capability.

Examples include:

- Test Performance
- PYQ Performance
- Answer Writing Performance
- Theme-wise Performance
- Strengths
- Weaknesses
- Readiness Indicators

The detailed information model will be defined in a future ADR.

---

# Inputs

Assessment Management consumes:

- Knowledge Assets
- Learning State
- Questions
- Tests
- Answer Writing
- Mock Examinations

---

# Outputs

Assessment Management produces:

- Performance Insights
- Learning Feedback
- Knowledge Feedback
- Improvement Opportunities
- Readiness Evaluation

---

# Architectural Principles

## Assessment is Feedback

Assessment exists to improve learning rather than merely measure it.

---

## Continuous Assessment

Assessment occurs throughout preparation and is not limited to examinations.

---

## Evidence-Based Evaluation

All assessment outcomes should be supported by observable learner performance.

---

## Separation of Concerns

Assessment evaluates learning.

It does not create knowledge or perform learning.

---

# Collaboration

Assessment Management collaborates with:

- Knowledge Management
- Learning Management
- Architecture Governance & Evolution

---

# Architecture Principle

> **Assessment transforms performance into actionable feedback for continuous improvement.**