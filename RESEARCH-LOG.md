# 📝 Research Log

## Session 1 — June 2026: Initial GitHub Discovery Sprint

### Methodology
- Searched GitHub using org-targeted queries: `org:CliMA`, `org:carbonplan`, `org:NOAA-GFDL`
- Supplemented with keyword searches: `climate geoengineering`, `solar radiation management`, `carbon capture`, `ocean intervention`
- Retrieved 15 most recent commits from top 3 active projects
- Evaluated activity by commit recency, star count, and update timestamps

### Projects Catalogued
- **Solar Geoengineering:** 6 projects
- **Carbon Capture:** 6 projects  
- **Ocean Intervention:** 5 projects
- **Total unique repos analyzed:** 17

### Key Observations
1. The **Julia language** has become dominant in next-generation climate modeling (CliMA ecosystem)
2. **Python/Jupyter** notebooks dominate the geoengineering-specific analysis tools (more accessible, less performant)
3. **Legacy Fortran** code (NOAA-GFDL) remains in institutional use but is not receiving new development
4. Most geoengineering-specific repos are **research artifacts** (low stars, inactive) rather than production tools
5. The gap between active **simulation infrastructure** (CliMA) and active **geoengineering application** code is significant — good podcast angle

### Activity Classification
| Status | Definition | Count |
|--------|-----------|-------|
| 🟢 Active | Commits within 30 days | 3 |
| 🟡 Maintained | Commits within 6 months | 3 |
| 🟠 Inactive | Last commit 6-24 months ago | 5 |
| 🔴 Deprecated | Formally deprecated | 1 |
| ❓ Unknown | Insufficient data | 5 |

### Next Research Steps
- [ ] Interview outreach: CliMA team (Gregory Wagner, Anna Jaruga)
- [ ] Interview outreach: CarbonPlan (Grayson Badgley, Oriana Chegwidden)
- [ ] Deep dive into CIDER emulator (Cornell) for solar episode
- [ ] Search for OAE-specific simulation tools (Planetary Technologies, etc.)
- [ ] Investigate CESM geoengineering scenario archive (NCAR)
- [ ] Review carbonplan/cdr-database methodology documentation
