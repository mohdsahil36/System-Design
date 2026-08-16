# LLD vs HLD

> **HLD** defines *what* the system looks like — architecture, components, and data flow
> **LLD** defines *how* the code is written — structure, patterns, and implementation details.

---

## Low-Level Design (LLD)

LLD is the blueprint for how code is written so it can be managed easily — not only by you, but by any developer who reads or maintains it. It focuses on **maintainable**, **extensible**, **testable**, and **understandable** code, guided by principles and design rules.

### Key questions LLD answers

| | Question |
|---|---|
| 1 | What code structure are we following? |
| 2 | What methods and APIs are being exposed? |
| 3 | How can we add new features without breaking existing code? |
| 4 | How do we keep the code testable and maintainable? |

**Focus areas:** classes · interfaces · design patterns · SOLID principles · code organization

---

## High-Level Design (HLD)

HLD is the architecture of the system. Once components are chosen based on requirements, HLD defines how they work together to achieve product goals — how data flows between them, how they communicate, and how the system stays **maintainable**, **reliable**, and **scalable**.

### Key questions HLD answers

| | Question |
|---|---|
| 1 | How is data being stored? |
| 2 | Do we need a cache? |
| 3 | How do we handle millions of users? |
| 4 | What happens if a service fails? |
| 5 | How do we handle scalability? |

**Focus areas:** services · databases · caching · load balancing · fault tolerance · APIs

---

## Quick comparison

| | **LLD** | **HLD** |
|---|---|---|
| **Scope** | Code & modules | System & infrastructure |
| **Audience** | Developers | Architects, tech leads, stakeholders |
| **Output** | Class diagrams, APIs, patterns | Architecture diagrams, data flow |
| **Thinks about** | *How* to write the code | *What* components exist & how they connect |
| **Example** | Strategy pattern for pricing logic | Redis cache in front of PostgreSQL |

---

## How they fit together

```text
Requirements
     ↓
   HLD  →  services, storage, scaling, failure handling
     ↓
   LLD  →  classes, methods, patterns, testability
     ↓
Implementation
```
