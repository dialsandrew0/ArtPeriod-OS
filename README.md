# ArtPeriod-OS

> Where art meets obsession. Honest deep analysis, observed-vs-inferred confidence, research index, and collection intelligence for collectors and field finds.

**ArtPeriod-OS** is the cleaned, production-focused evolution of the ArtPeriod line and ArtPeriod Field Triage. It serves two complementary modes:

1. **Field / Estate mode** — rapid, honest triage of unknown or mid-market works found at sales and auctions.
2. **Collection & Research mode** — tracking, revaluation where data exists, and a research index grounded in open collections + authority sources.

The non-negotiable principle: **be trustworthy about what the system knows versus what it is guessing**.

---

## Core Principles

- **Observed vs Inferred** on every analysis
- Confidence scores with reasons and evidence
- Prefer “insufficient data” over false precision
- Open-collection research index (Met CC0 and similar) + authority resolution (Wikidata, Getty ULAN, etc.)
- Collection dashboard that does not require museum-level data to be useful

---

## Product Surfaces

### Field Triage
Photograph a piece → structured card:
- Observed (medium, marks, condition, visible signatures/labels)
- Inferred (period, school, possible maker, value band) with confidence
- Physical checks still required before purchase
- Sources when available

### Research Index
Local or hosted embedding-searchable mirror of open collections + artist authority resolution + visual match tiers. Designed for desk research, not field speed.

### Collection Intelligence
Track works you own or watch. Continuous revaluation only where comparable data exists; clear gaps otherwise. No invented numbers.

---

## Customer Personas

1. **Field collector / dealer** who finds works at estates and auctions  
   Needs fast, honest triage rather than blue-chip-only tools.

2. **Serious mid-market collector**  
   Needs collection tracking and realistic market signals without enterprise pricing or opacity.

3. **Researcher / appraiser assistant**  
   Needs a grounded research index with clear provenance of data.

---

## Architecture (target)

```
ArtPeriod-OS/
├── apps/
│   ├── field/              # Fast triage experience (mobile-first)
│   └── collection/         # Dashboard + research
├── packages/
│   ├── honesty/            # Observed / Inferred / Confidence schemas
│   ├── research-index/     # Embeddings, authority resolution, visual match
│   └── shared/
├── data/                   # Open collection ingestion notes & licenses
└── docs/
    ├── HONESTY.md
    ├── DATA-SOURCES.md
    ├── PERSONAS.md
    └── ROADMAP.md
```

Tech direction: Next.js / TypeScript, Prisma or equivalent, strong typing on honesty layer, careful handling of open vs gated data licenses.

---

## Market Position

Heavy platforms (Artnet, Artsy, Artprice, MutualArt, LiveArt, Art Collector IQ) dominate blue-chip auction results and indices. They are weaker on:
- Unknown / mid-tier / field-found works
- Explicit confidence and evidence
- Tools optimized for the person standing in an estate sale

ArtPeriod-OS owns the honesty + field + mid-market + research-index combination.

---

## Reality Check & Next Moves

**Carried forward**  
- Observed vs Inferred philosophy from Field Triage  
- Research index spine  
- Collection + discovery roadmap from earlier ArtPeriod work

**Gaps**  
- Clean single codebase (multiple prior variants exist)  
- Production research index with real open data  
- Cost controls on vision/LLM  
- Clear licensing and attribution for every data source

**Immediate roadmap**  
1. Lock honesty schemas and make them the foundation of every analysis surface  
2. Port and harden the best Field Triage card experience  
3. Stand up a minimal research index with Met CC0 (or equivalent) sample  
4. Collection tracker MVP with honest “no data” states  
5. Private feedback from collectors and field dealers

---

## Brand & Naming Note

This repository is the canonical **ArtPeriod-OS**. Prior variants (`artperiod`, `ArtPeriodt`, `ART-period-`, `ArtPeriodFieldTriage`, etc.) should be treated as historical. New development and public positioning use **ArtPeriod-OS**.

Honesty first. Obsession second. Results third.
