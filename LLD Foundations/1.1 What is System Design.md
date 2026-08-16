# What is System Design?

> The process of defining a system's elements, their relationships, and how they communicate — to solve a given problem statement.

---

## Definition

System design is the process of defining the elements of a system, as well as their relationships with each other and the communication between them, so that we can work around a problem statement.

---

## What it involves

| Step | Activity |
|:---:|---|
| 1 | Break down the system into sub-components / parts |
| 2 | Design each part to satisfy the problem statement & product requirements |
| 3 | Find loopholes or deficiencies in the current setup |
| 4 | Fix and optimize issues for better performance & business requirements |
| 5 | **Iterate** — design → fix → test → repeat |

---

## The design loop

```text
  ┌──────────┐
  │  Design  │
  └────┬─────┘
       ↓
  ┌──────────┐     ┌──────────┐
  │   Fix    │ ←── │   Test   │
  └────┬─────┘     └────▲─────┘
       └────────────────┘
            repeat
```

**Goal:** a system that meets requirements today and can evolve as those requirements change.
