# Communication overhead · Clubhub--Team3 (v1.0, 2026-10-20)

## Paths

Using the formula $P = \frac{n(n-1)}{2}$ to calculate total communication channels/paths:

* **Model (a) - Everyone + Client:** 4 team members + 1 Client = 5 people ($n = 5$).
  $$\text{Paths} = \frac{5 \times (5 - 1)}{2} = \frac{20}{2} = 10 \text{ paths}$$
* **Model (b) - Client via PO:** 4 team members intercommunicating ($n = 4$) plus 1 path between PO and Client.
  $$\text{Paths} = \frac{4 \times (4 - 1)}{2} + 1 = \frac{12}{2} + 1 = 6 + 1 = 7 \text{ paths}$$

| Model | People n | Paths n(n-1)/2 | Minutes/week | Hours/week |
|-------|----------|----------------|--------------|------------|
| (a) everyone + client | 5 | 10 | 100 | 1.67 |
| (b) client via PO | 5 | 7 | 70 | 1.17 |

**Assumption:** 10 minutes per path per week, because each pairwise sync/alignment requires short weekly updates and status checks.
**Team capacity:** 4 members × 6 h = 24 h/week -> overhead = **4.9%** of weekly capacity for Model (b).

## Our paths (model b)

```mermaid
flowchart LR
   Client --- Naihouy
   Naihouy ---  Setha
   Naihouy --- kimseng
   Naihouy --- Sekang
   Setha --- kimseng
   Setha ---  Sekang
   kimseng --- Sekang

## Two practices

1. GitHub Issues as the single source of truth: Replaces scatterd chat arguments with structured traking, reducing conversational paths.
  New estimated overhead 50min/0.83h/week
2. Weekly 15-minutes Stand up: Restrcts full-team syncs to a strict, timeboxed interval instead of ad-hoc meeting 
  New estimate overhead 40 min/ 0.67h /week

## A sixth member in week 11?
Adding a 6th member in week 11 increases model (b) paths to 12 ($5 \times 4 / 2 + 1$), spiking communication overhead right when the team needs to be coding during Sprint 1; therefore, according to Brooks's law, we would **decline** adding a member so late in the project.

## Reflection: the essential difficulty we expect first
Our team expects to hit **complexity** first in ITC Club Hub [cite: [Lab-01 · Software Development Challenges](https://gicitc.com/courses/introduction-to-software-engineering/01-SoftwareDevelopmentChallenges/Lab-01.html?continue#challenge-communication-overhead)]. For example, managing overlapping business rules between student registrations, capacities, and cancellation deadlines will quickly tangle our code logic. Over the next four weeks, we will counter this by strictly separating our domain logic into clean C++ classes and enforcing thorough peer code reviews on every pull request.
-  (signed) Naihouy, 2026-10-20
-  (signed)Setha, 2026-10-20
-  (signed) kimseng, 2026-10-20
-  Sekang, 2026-10-20
