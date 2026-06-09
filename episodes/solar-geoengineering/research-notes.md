# 🌞 Episode Research: Solar Geoengineering

> **Podcast Series:** Climate Technology & Geoengineering  
> **Branch:** `solar-geoengineering`  
> **Last Updated:** June 2026  
> **Status:** Active Research

---

## 📌 Episode Overview

This episode covers **Solar Radiation Management (SRM)** — the class of geoengineering techniques that aim to reduce incoming solar radiation to cool the Earth. Key subtopics include Stratospheric Aerosol Injection (SAI), Marine Cloud Brightening (MCB), and space-based reflectors. The open-source community is developing increasingly sophisticated simulation tools to model these interventions.

---

## 🔭 Key GitHub Projects Discovered

### 1. [CliMA/ClimaAtmos.jl](https://github.com/CliMA/ClimaAtmos.jl)
- **Stars:** 119 ⭐ | **Language:** Julia | **Status:** 🟢 EXTREMELY ACTIVE
- **Description:** The Climate Modelling Alliance's (CliMA) atmosphere model, designed to leverage data assimilation and machine learning for modeling and calibrating subgrid-scale processes.
- **Relevance to Solar Geoengineering:** Models atmospheric radiative transfer, albedo feedback, and cloud microphysics — all critical for simulating SAI and MCB scenarios. Recent work on `CouplerAlbedo` directly relevant.
- **Notable:** Uses GPU acceleration for high-resolution global simulations.

### 2. [CliMA/Insolation.jl](https://github.com/CliMA/Insolation.jl)
- **Stars:** 17 ⭐ | **Language:** Julia | **Status:** 🟡 MAINTAINED
- **Description:** Calculates solar radiation and solar geometry, including solar zenith angle, azimuth angle, and incoming solar radiation (insolation) at any point on Earth.
- **Relevance:** Core library for computing the baseline solar forcing that geoengineering interventions would modify. Essential dependency for any SRM simulation.
- **Last Updated:** May 2026

### 3. [ClimateMARGO/ClimateMARGO.jl](https://github.com/ClimateMARGO/ClimateMARGO.jl)
- **Stars:** 73 ⭐ | **Language:** Julia | **Status:** 🟠 INACTIVE (last commit Oct 2023)
- **Description:** Julia implementation of MARGO — an idealized climate-economic modelling framework for optimizing trade-offs between **M**itigation, **A**daptation, carbon **R**emoval, and **G**eo-engineering **O**ptions.
- **Relevance:** Directly models geoengineering as one of four climate levers. Useful for economic framing of solar geoengineering debates.
- **Notable:** Includes Pluto.jl interactive notebooks for visualization.

### 4. [JdeJong96/sai-git](https://github.com/JdeJong96/sai-git)
- **Stars:** — | **Language:** Jupyter Notebook | **Status:** 🟠 INACTIVE (last commit Aug 2025)
- **Description:** Tools for analyzing CESM (Community Earth System Model) geoengineering climate data, specifically focused on Stratospheric Aerosol Injection scenarios.
- **Relevance:** Direct SAI analysis tooling built on top of NCAR's CESM model output.

### 5. [jf678-cornell/CIDER](https://github.com/jf678-cornell/CIDER)
- **Stars:** 4 ⭐ | **Language:** Jupyter Notebook | **Status:** 🟡 RECENT (last commit March 2026)
- **Description:** The **C**limate **I**ntervention **D**ynamical **E**mula**t**o**R** — a lightweight, reduced-order model for exploring highly dynamic geoengineering scenarios.
- **Relevance:** Emulator approach allows rapid prototyping of geoengineering scenarios without running full Earth System Models. Important for sensitivity analysis.

### 6. [alistairduffey/Geoengineering_toy_model](https://github.com/alistairduffey/Geoengineering_toy_model)
- **Stars:** — | **Language:** Jupyter Notebook
- **Description:** Simple model of the global climate response to emissions and geoengineering interventions.
- **Relevance:** Educational/accessible entry point for understanding feedback mechanisms.

---

## 📊 Commit Trend Analysis: CliMA/ClimaAtmos.jl

> **Verdict: 🔥 Blazing Active — Multiple commits daily in June 2026**

| Date | Commit | Author | Significance |
|------|--------|--------|--------------|
| Jun 9, 2026 | Update to ClimaCore 0.14.54 | Nat Efrat-Henrici | Dependency modernization |
| Jun 8, 2026 | Docs: reorganize structure & improve getting-started | Haakon Ervik | Developer onboarding push |
| Jun 8, 2026 | Tag patch release | Nat Efrat-Henrici | v0.x.x release cycle |
| Jun 5, 2026 | Add new alloc test (EDMF 1M) | Anna Jaruga | Performance benchmarking |
| Jun 5, 2026 | Remove q_tot diffusion contribution to updraft area tendency | Sajjad Azimi | **Microphysics refinement** |
| Jun 5, 2026 | Add consistent non-eq microphysics + cloud fraction (truncated gaussian) | Sajjad Azimi | **Cloud physics advance** |
| Jun 4, 2026 | Clean up accumulation of available configs | Dennis Yatunin | Infrastructure improvement |
| Jun 4, 2026 | Microphysics tendency output | Anna Jaruga | **Diagnostic enhancement** |
| Jun 4, 2026 | Initialize albedo as NaN for CouplerAlbedo | Julia Sloan | **Albedo coupling fix** |

### 🔍 Trend Summary
- **Cloud microphysics** is the dominant area of development — directly relevant to Marine Cloud Brightening modeling.
- **EDMF (Eddy-Diffusivity Mass-Flux) turbulence scheme** is being actively refined, improving how the model handles convection and aerosol transport.
- **CouplerAlbedo** work signals integration between atmosphere and surface albedo models — key for SRM scenario testing.
- **Documentation push** in early June suggests the project is maturing and seeking broader adoption.
- Active contributors: Anna Jaruga, Sajjad Azimi, Dennis Yatunin, Julia Sloan, Haakon Ervik.

---

## 🎙️ Podcast Angle Ideas

1. **"The Code Behind the Aerosol Veil"** — How ClimaAtmos.jl models stratospheric aerosol injection; interview with Anna Jaruga on microphysics.
2. **"Sun Dimming on a Budget"** — CIDER emulator as a democratizing tool for geoengineering research without supercomputers.
3. **"The MARGO Dilemma"** — Using ClimateMARGO.jl to illustrate the economic trade-offs of deploying solar geoengineering vs. mitigation.
4. **"Who Gets to Dim the Sun?"** — Governance angle using open-source transparency as a frame.

---

## 📚 Key Terms for Episode

- **SAI** — Stratospheric Aerosol Injection
- **MCB** — Marine Cloud Brightening
- **SRM** — Solar Radiation Management
- **CESM** — Community Earth System Model (NCAR/UCAR)
- **EDMF** — Eddy-Diffusivity Mass-Flux (turbulence parameterization)
- **Radiative Forcing** — Change in energy flux from interventions
- **Termination Shock** — Sudden warming if SAI deployment is stopped

---

## 🔗 Further Resources

- [CliMA Organization on GitHub](https://github.com/CliMA)
- [SCoPEx Project (Harvard)](https://projects.iq.harvard.edu/keutschgroup/scopex)
- [NOAA Geoengineering Research](https://www.noaa.gov)
- [Silver Lining NGO](https://www.silverlining.ngo)
