# Graph Report - bgs4who  (2026-11-05)

## Corpus Check
- 2 files · ~288,324 words
- Verdict: corpus is large enough that graph structure adds value.

## Summary
- 30 nodes · 28 edges · 6 communities
- Extraction: 100% EXTRACTED · 0% INFERRED · 0% AMBIGUOUS
- Token cost: 0 input · 0 output

## Graph Freshness
- Built from commit: `02c469f5`
- Run `git rev-parse HEAD` and compare to check if the graph is stale.
- Run `graphify update .` after code changes (no API cost).

## Community Hubs (Navigation)
- [[_COMMUNITY_Community 0|Community 0]]
- [[_COMMUNITY_Community 1|Community 1]]
- [[_COMMUNITY_Community 2|Community 2]]
- [[_COMMUNITY_Community 3|Community 3]]
- [[_COMMUNITY_Community 4|Community 4]]
- [[_COMMUNITY_Community 5|Community 5]]

## God Nodes (most connected - your core abstractions)
1. `antislop audit 001 — 2026-09-19` - 6 edges
2. `antislop audit 002 — 2026-09-19` - 6 edges
3. `Fixed` - 5 edges
4. `Resolved by written reason, no visual change` - 5 edges
5. `MEDIUM — Purpose-Gate` - 4 edges
6. `LOW — Quality Locks` - 4 edges
7. `HIGH — Hard Gate` - 3 edges
8. `1. R-25 — Hero text fails WCAG AA at every breakpoint` - 1 edges
9. `2. R-02 — Seven em dashes` - 1 edges
10. `3. C-4 / R-35 — Cloudflare challenge script left in the mirror` - 1 edges

## Surprising Connections (you probably didn't know these)
- None detected - all connections are within the same source files.

## Communities (6 total, 0 thin omitted)

### Community 0 - "Community 0"
Cohesion: 0.29
Nodes (6): 1. R-25 — Hero text fails WCAG AA at every breakpoint, 2. R-02 — Seven em dashes, antislop audit 001 — 2026-09-19, HIGH — Hard Gate, Not verified, Passes (with evidence)

### Community 1 - "Community 1"
Cohesion: 0.40
Nodes (4): antislop audit 002 — 2026-09-19, Click-through evidence (R-35), Delivery Gate, Remaining

### Community 2 - "Community 2"
Cohesion: 0.40
Nodes (5): 1. R-25 — Hero contrast (was FAIL at every breakpoint) — FIXED, 2. R-02 — Em dashes — FIXED, 3. C-4 / R-35 — Cloudflare challenge script — FIXED, 6. R-32 — Focus indicator — FIXED, Fixed

### Community 3 - "Community 3"
Cohesion: 0.40
Nodes (5): 4. R-14 — Identical feature cards — ACCEPTED WITH REASON, 5. R-06 — Typography — SUPERSEDED, 7. R-37 / R-31 — Direction — FIXED, 8. R-29 — Palette — DOCUMENTED, Resolved by written reason, no visual change

### Community 4 - "Community 4"
Cohesion: 0.50
Nodes (4): 3. C-4 / R-35 — Cloudflare challenge script left in the mirror, 4. R-14 — Identical feature cards, 5. R-06 — `Inter` is never loaded, MEDIUM — Purpose-Gate

### Community 5 - "Community 5"
Cohesion: 0.50
Nodes (4): 6. R-32 — No explicit focus indicator, 7. R-37 / R-31 — Direction not written down, 8. R-29 — Palette size not declared, LOW — Quality Locks

## Knowledge Gaps
- **21 isolated node(s):** `1. R-25 — Hero text fails WCAG AA at every breakpoint`, `2. R-02 — Seven em dashes`, `3. C-4 / R-35 — Cloudflare challenge script left in the mirror`, `4. R-14 — Identical feature cards`, `5. R-06 — `Inter` is never loaded` (+16 more)
  These have ≤1 connection - possible missing edges or undocumented components.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `antislop audit 001 — 2026-09-19` connect `Community 0` to `Community 4`, `Community 5`?**
  _High betweenness centrality (0.187) - this node is a cross-community bridge._
- **Why does `antislop audit 002 — 2026-09-19` connect `Community 1` to `Community 2`, `Community 3`?**
  _High betweenness centrality (0.175) - this node is a cross-community bridge._
- **Why does `Fixed` connect `Community 2` to `Community 1`?**
  _High betweenness centrality (0.113) - this node is a cross-community bridge._
- **What connects `1. R-25 — Hero text fails WCAG AA at every breakpoint`, `2. R-02 — Seven em dashes`, `3. C-4 / R-35 — Cloudflare challenge script left in the mirror` to the rest of the system?**
  _21 weakly-connected nodes found - possible documentation gaps or missing edges._