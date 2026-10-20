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