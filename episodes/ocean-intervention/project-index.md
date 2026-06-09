# Ocean Intervention — Project Quick Reference

| Project | Org | Stars | Language | Activity | Focus |
|---------|-----|-------|----------|----------|-------|
| Oceananigans.jl | CliMA | 1,333 | Julia | 🟢 Daily | Ocean fluid dynamics & tracer transport |
| OceanParameterizations.jl | CliMA | 22 | Julia | 🟡 Maintained | ML for ocean mixing parameterization |
| ClimaLand.jl | CliMA | 71 | Julia | 🟢 Active | Land/coastal/blue carbon modeling |
| SM2 | NOAA-GFDL | 1 | Fortran | 🔵 Institutional | Slab ocean model (legacy) |
| ClimateMachine.jl | CliMA | 470 | Julia | 🔴 Deprecated | Original ESM (now split into modules) |

> 💡 **Key Insight:** Oceananigans.jl is the clear standout — with 1,333 stars and near-daily commits, it is the most actively developed open-source ocean simulation framework in the world. Its June 2026 development sprint on TripolarGrid, Zarr I/O, and tracer boundary conditions positions it as the go-to tool for ocean intervention impact modeling.

## 📊 Commit Velocity Comparison

```
Project                    Commits/Month (Jun 2026)   Trend
Oceananigans.jl            ~20-25                     📈 Accelerating
ClimaLand.jl               ~10-15                     📈 Growing
OceanParameterizations.jl  ~2-3                       ➡️  Steady
SM2 (NOAA-GFDL)            ~0-1                       📉 Minimal
ClimateMachine.jl          0 (deprecated)             ⛔ Stopped
```

## 🌊 Ocean Intervention Technology Landscape

```
High Maturity  │ Low Maturity
───────────────┼──────────────────────────────
OAE modeling   │ Artificial upwelling sims
Iron fert. sims│ Seaweed CDR quantification  
Blue carbon    │ Deep ocean CO₂ injection
Heat uptake    │ Coastal brightening
```
