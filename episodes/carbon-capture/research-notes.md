# 🌱 Episode Research: Carbon Capture

> **Podcast Series:** Climate Technology & Geoengineering  
> **Branch:** `carbon-capture`  
> **Last Updated:** June 2026  
> **Status:** Active Research

---

## 📌 Episode Overview

This episode covers **Carbon Dioxide Removal (CDR)** — the family of technologies and approaches designed to remove CO₂ directly from the atmosphere or point sources. This spans Direct Air Capture (DAC), Bioenergy with Carbon Capture and Storage (BECCS), enhanced weathering, forest carbon markets, and soil carbon sequestration. Open-source tools are increasingly central to evaluating CDR claims and modeling carbon cycles.

---

## 🔭 Key GitHub Projects Discovered

### 1. [carbonplan/cdr-database](https://github.com/carbonplan/cdr-database)
- **Stars:** 29 ⭐ | **Language:** JavaScript | **Status:** 🟡 MAINTAINED
- **Description:** A public database of reports on carbon removal projects and technologies, covering permanence, additionality, co-benefits, and risks.
- **Relevance:** The most comprehensive open-source CDR project evaluation framework publicly available. CarbonPlan has become the de facto independent auditor of voluntary carbon markets.
- **Last Updated:** Dec 2025
- **Notable:** Backed by peer-reviewed methodology; widely cited in policy documents.

### 2. [carbonplan/forest-risks](https://github.com/carbonplan/forest-risks)
- **Stars:** 35 ⭐ | **Language:** Jupyter Notebook | **Status:** 🟠 INACTIVE (last meaningful commit Nov 2022)
- **Description:** Statistical models of forest carbon potential and risks, including wildfire, drought, and pest-driven carbon loss scenarios.
- **Relevance:** Directly challenges the permanence assumptions of forest-based carbon offsets. The models here were used in landmark papers questioning California's forest carbon buffer pool.
- **Key Finding:** Forest carbon offsets are far riskier under climate change than offset registries account for.

### 3. [carbonplan/carbonplan-buffer-analysis](https://github.com/carbonplan/carbonplan-buffer-analysis)
- **Stars:** 4 ⭐ | **Language:** Python
- **Description:** Quantitative analysis of the risks to the California forest carbon buffer pool.
- **Relevance:** Specific policy-relevant analysis showing the California Air Resources Board's offset buffer pool is severely under-reserved for climate risk.

### 4. [ClimateMARGO/ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl)
- **Stars:** 73 ⭐ | **Language:** Julia | **Status:** 🟠 INACTIVE (last commit Oct 2023)
- **Description:** MARGO framework includes **carbon Removal** (R) as one of four climate levers alongside Mitigation, Adaptation, and Geoengineering.
- **Relevance:** Allows modeling of CDR deployment rates and costs within an integrated climate-economic framework. Useful for illustrating the scale of CDR needed under different emissions pathways.

### 5. [KOSASIH/GCCS-Core](https://github.com/KOSASIH/GCCS-Core)
- **Stars:** 9 ⭐ | **Language:** Python
- **Description:** Global Climate Control System — foundational framework encompassing core algorithms, data management, and integration components for a comprehensive climate control system.
- **Relevance:** Ambitious open-source attempt at a unified climate intervention management system. Useful as an example of community-driven CDR integration thinking.

### 6. [CliMA/ClimaLand.jl](https://github.com/CliMA/ClimaLand.jl)
- **Stars:** 71 ⭐ | **Language:** Julia | **Status:** 🟢 ACTIVE (updated June 2026)
- **Description:** CliMA's land model, simulating soil, vegetation, and land-surface processes.
- **Relevance:** Land surface models are essential for quantifying natural carbon sinks (forests, soils) and evaluating nature-based CDR solutions like afforestation and soil carbon enhancement.

---

## 📊 Commit Trend Analysis: carbonplan/forest-risks

> **Verdict: 🟠 Mostly Dormant — Research phase complete, awaiting policy uptake**

| Date | Commit | Author | Significance |
|------|--------|--------|--------------|
| Jan 11, 2024 | Update pre-commit hooks | Max Jones | Minor maintenance |
| Jan 10, 2024 | Update badges, monogram, grammar | Max Jones | Documentation polish |
| Nov 23, 2022 | Merge datasets PR | Anderson Banihirwe | Dataset documentation |
| Nov 22, 2022 | Update datasets.md | Oriana Chegwidden | Data provenance |
| Nov 22, 2022 | List of datasets for forest risks | Oriana | **Core dataset release** |
| Oct 24, 2022 | Update README | Kata Martin | Documentation |

### 🔍 Trend Summary
- The project entered **maintenance mode** after its landmark 2022 publication period.
- The core scientific work (statistical models, risk quantification) appears **complete and published**.
- Activity pattern is typical of **research-to-publication** repositories: intense development, then freeze.
- The codebase is being preserved rather than extended — suggesting the findings have been incorporated into CarbonPlan's broader tooling.
- **Key Implication for Podcast:** The forest carbon offset market critique is now well-documented and the code is auditable by anyone — a powerful transparency story.

---

## 📊 Commit Trend Analysis: CliMA/ClimaLand.jl

> **Verdict: 🟢 Active — Land carbon modeling advancing alongside atmosphere work**

- Updated June 8, 2026 — in sync with the broader CliMA ecosystem
- Part of the tightly coupled CliMA Earth System Model development sprint
- Soil and vegetation carbon parameterizations being refined to match ClimaAtmos.jl coupling

---

## 🎙️ Podcast Angle Ideas

1. **"The Carbon Offset Audit"** — How CarbonPlan used open-source code to expose weaknesses in the voluntary carbon market; interview with Grayson Badgley or Oriana Chegwidden.
2. **"DAC: The $1,000 Per Ton Question"** — Explore the economics of Direct Air Capture using MARGO's cost curves; what does open-source modeling say about DAC scalability?
3. **"Forests Can't Save Us Alone"** — Deep dive into forest-risks findings; why permanence is the Achilles heel of nature-based solutions.
4. **"The Land Model Gap"** — Why soil carbon is the least-understood component of the carbon cycle and how ClimaLand.jl is trying to fix that.

---

## 📚 Key Terms for Episode

- **DAC** — Direct Air Capture (mechanical CO₂ removal)
- **BECCS** — Bioenergy with Carbon Capture and Storage
- **CDR** — Carbon Dioxide Removal
- **Permanence** — How long captured carbon stays out of the atmosphere
- **Additionality** — Whether carbon removal would have happened anyway
- **Buffer Pool** — Reserve credits held against future carbon losses in offset projects
- **Leakage** — Emissions displaced rather than reduced
- **Enhanced Weathering** — Spreading crushed silicate rock to accelerate natural CO₂ absorption

---

## 🔗 Further Resources

- [CarbonPlan](https://carbonplan.org) — Independent CDR analysis
- [Carbon180](https://carbon180.org) — CDR policy advocacy
- [Project Drawdown](https://drawdown.org) — Ranked CDR solutions
- [IPCC AR6 Chapter 12](https://www.ipcc.ch/ar6) — CDR mitigation pathways
- [Global CCS Institute](https://www.globalccsinstitute.com)
