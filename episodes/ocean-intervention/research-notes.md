# 🌊 Episode Research: Ocean Intervention

> **Podcast Series:** Climate Technology & Geoengineering  
> **Branch:** `ocean-intervention`  
> **Last Updated:** June 2026  
> **Status:** Active Research

---

## 📌 Episode Overview

This episode covers **Ocean-Based Climate Interventions** — a rapidly growing field that leverages the ocean's enormous capacity to absorb heat and CO₂. Techniques include Ocean Alkalinity Enhancement (OAE), Iron Fertilization, Seaweed/Kelp Cultivation for carbon sequestration, and Artificial Upwelling. The ocean covers 71% of Earth's surface and has absorbed ~90% of excess heat from climate change, making it both a victim of and potential solution to the climate crisis.

---

## 🔍 Key GitHub Projects Discovered

### 1. [CliMA/Oceananigans.jl](https://github.com/CliMA/Oceananigans.jl)
- **Stars:** 1,333 ⭐ | **Language:** Julia | **Status:** 🟢 FLAGSHIP ACTIVE PROJECT
- **Description:** Fast, friendly, flexible ocean-flavored fluid dynamics on CPUs and GPUs. The leading open-source ocean simulation framework in the Julia ecosystem.
- **Relevance:** The foundational simulation engine for modeling ocean circulation, mixing, and tracer transport — all essential for evaluating ocean intervention scenarios including alkalinity plume dispersal, iron fertilization transport, and heat/CO₂ uptake.
- **Notable Features:** GPU acceleration (NVIDIA CUDA, AMD ROCm), distributed computing, immersed boundary methods for complex bathymetry, Zarr I/O for cloud-native data.
- **Scale:** Can run from idealized 2D experiments to global ocean simulations.

### 2. [CliMA/OceanParameterizations.jl](https://github.com/CliMA/OceanParameterizations.jl)
- **Stars:** 22 ⭐ | **Language:** Julia | **Status:** 🟡 MAINTAINED
- **Description:** Machine learning and uncertainty quantification for climate model parameterizations using differentiable and probabilistic programming.
- **Relevance:** Addresses one of the biggest challenges in ocean intervention modeling: subgrid-scale mixing processes that determine how interventions (alkalinity, iron) actually disperse in the real ocean.
- **Last Updated:** Feb 2026

### 3. [NOAA-GFDL/SM2](https://github.com/NOAA-GFDL/SM2)
- **Stars:** 1 ⭐ | **Language:** Fortran | **Status:** 🔵 INSTITUTIONAL
- **Description:** GFDL Slab Ocean Model — NOAA's Geophysical Fluid Dynamics Laboratory ocean component.
- **Relevance:** Represents the institutional/operational side of ocean climate modeling. Fortran-based legacy code that powers NOAA's operational forecasting.
- **Notable:** Contrast with Oceananigans.jl illustrates the generational shift happening in climate computing.

### 4. [CliMA/ClimaLand.jl](https://github.com/CliMA/ClimaLand.jl)
- **Stars:** 71 ⭐ | **Language:** Julia | **Status:** 🟢 ACTIVE
- **Description:** CliMA's land model — includes coastal and wetland processes relevant to blue carbon.
- **Relevance:** Coastal wetlands (mangroves, salt marshes, seagrasses) are among the most carbon-dense ecosystems on Earth. Blue carbon sequestration is increasingly considered a nature-based ocean intervention.

### 5. [CliMA/ClimateMachine.jl](https://github.com/CliMA/ClimateMachine.jl) ⚠️ DEPRECATED
- **Stars:** 470 ⭐ | **Language:** Julia | **Status:** 🔴 DEPRECATED
- **Description:** The original CliMA Earth System Model. Now carries a deprecation notice; functionality has been split into the modular ClimaAtmos.jl, Oceananigans.jl, and ClimaLand.jl.
- **Relevance:** Historical context — represents the architectural evolution from monolithic to modular climate modeling. Last real commits in 2021.
- **Podcast Angle:** The deprecation story illustrates how the field is maturing and adopting software engineering best practices.

---

## 📊 Commit Trend Analysis: CliMA/Oceananigans.jl

> **Verdict: 🔥 Most Active Ocean Simulation Project on GitHub — Multiple commits per week in June 2026**

| Date | Commit | Author | Significance |
|------|--------|---------|--------------|
| Jun 8, 2026 | Add ::Nothing methods to avoid type piracy | Navid C. Constantinou | **API stability & composability** |
| Jun 7, 2026 | Update cell_diffusion_timescale for vertically-implicit treatment | Navid C. Constantinou | **Numerical solver improvement** |
| Jun 6, 2026 | Add inactive_nodes to NetCDFWriter's gather_immersed_boundary | Tomás Chor | **Bathymetry output fix** |
| Jun 3, 2026 | Update Project.toml | Gregory L. Wagner | Dependency management |
| Jun 3, 2026 | Allow set! to copy between reduced and windowed single-layer fields | Gregory L. Wagner | **Field manipulation API** |
| Jun 2, 2026 | Add target_transport to PerturbationAdvection for per-boundary transport control | Tomás Chor | **Boundary condition flexibility** |
| Jun 2, 2026 | (0.110.0) Rename Open → NormalFlow and add a scheme to Value | Gregory L. Wagner | **Boundary condition redesign** |
| Jun 1, 2026 | Add Zarr writer and chunk size as option to IO benchmark | David Kamm | **Cloud-native I/O** |
| Jun 1, 2026 | Apply tracer open boundary conditions in NonhydrostaticModel | Tomás Chor | **Tracer transport** |
| May 29, 2026 | Fix _fractional_indices ambiguities and adapt last_Δt | dkytezab | Numerical precision |
| May 28, 2026 | Regularize correctly U and V bc for TripolarGrid | Simone Silvestri | **Global grid support** |
| May 28, 2026 | Support tracers in PerturbationAdvection open boundary conditions | Tomás Chor | **Tracer boundary conditions** |
| May 27, 2026 | Bump version 0.108.1 → 0.109.0 | dkytezab | Minor version release |

### 🔍 Trend Summary

**Dominant Development Themes (June 2026):**

1. **🌐 Global Ocean Grids** — TripolarGrid support (May 28) signals a push toward global-scale simulations, not just regional models. This is the foundation for global ocean intervention impact assessments.

2. **🏔️ Immersed Boundary Methods** — Ongoing work on `gather_immersed_boundary` enables realistic complex seafloor topography (seamounts, continental shelves) — critical for modeling how alkalinity disperses near coastlines.

3. **☁️ Cloud-Native I/O** — Zarr writer addition (Jun 1) is a major shift enabling petabyte-scale ocean simulation output to be stored and processed in cloud environments (AWS, GCS). This democratizes access to large simulation datasets.

4. **🌊 Boundary Condition Overhaul** — The rename of `Open → NormalFlow` and the `PerturbationAdvection` work (Jun 2) represent a significant boundary condition API redesign, improving how ocean models handle open boundaries and tracer fluxes — directly relevant to modeling how interventions enter and leave a domain.

5. **🧪 Tracer Transport** — Multiple commits on tracer boundary conditions and transport suggest active development of the chemical tracer infrastructure needed to model alkalinity, iron, and CO₂ plumes.

**Active Core Contributors:** Gregory L. Wagner, Navid C. Constantinou, Tomás Chor, Simone Silvestri, David Kamm

---

## 🎙️ Podcast Angle Ideas

1. **"The Ocean as a Carbon Sponge"** — How Oceananigans.jl models the ocean's natural carbon uptake and what happens when we try to enhance it; interview with Gregory L. Wagner (MIT/CliMA).
2. **"Alkalinity: Turning the Ocean into Limestone"** — Ocean Alkalinity Enhancement deep dive; how the tracer transport work in Oceananigans.jl enables OAE impact modeling.
3. **"Iron Fertilization: Bloom or Bust?"** — History of iron fertilization experiments (LOHAFEX, SOIREE) and what modern open-source models tell us about scalability.
4. **"From Fortran to Julia: The Great Climate Computing Migration"** — The story of NOAA-GFDL/SM2 vs. Oceananigans.jl as a metaphor for the generational shift in climate science software.
5. **"Blue Carbon's Promise"** — Mangroves, seagrasses, and kelp forests as ocean-based CDR; how ClimaLand.jl is beginning to model coastal carbon stocks.

---

## 📚 Key Terms for Episode

- **OAE** — Ocean Alkalinity Enhancement (adding alkaline minerals to increase CO₂ absorption)
- **Iron Fertilization** — Adding iron to HNLC (High Nutrient, Low Chlorophyll) ocean regions to stimulate phytoplankton blooms
- **HNLC** — High Nutrient, Low Chlorophyll zones where iron limits biological productivity
- **Blue Carbon** — Carbon stored in coastal marine ecosystems (mangroves, seagrasses, salt marshes)
- **Biological Pump** — The ocean's natural mechanism for transporting surface carbon to the deep ocean
- **Thermohaline Circulation** — The global ocean conveyor belt driven by temperature and salinity differences
- **Meso-scale Eddies** — Ocean vortices 10-100km in diameter that drive much of the ocean's heat and tracer transport
- **Artificial Upwelling** — Using pipes or pumps to bring cold, nutrient-rich deep water to the surface
- **TripolarGrid** — A numerical grid for global ocean modeling that avoids singularities at the poles

---

## 🔗 Further Resources

- [CliMA/Oceananigans.jl Documentation](https://clima.github.io/OceananigansDocumentation/stable/)
- [NOAA GFDL Ocean Research](https://www.gfdl.noaa.gov/ocean/)
- [Ocean Visions CDR Roadmaps](https://oceanvisions.org)
- [MBARI Ocean CDR Research](https://www.mbari.org)
- [Planetary Technologies (OAE startup)](https://www.planetarytech.com)
- [Running Tide (kelp CDR)](https://www.runningtide.com)
