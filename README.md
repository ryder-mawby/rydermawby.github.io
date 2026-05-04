# Ryder Mawby

**Empirical Economist · Illicit Market Geography · Cryptomarket Data**

MA Economics, California State University, Long Beach (Expected December 2026)  
BA Political Economy, UC Berkeley (Regents’ Scholar, 2023)  
Contact: rydermawby@berkeley.edu

---

## About

This repository supports my research on illicit markets, with a focus on
the geography of darknet cryptomarket trade and the application of
structural gravity models to non-traditional economic systems.

My work uses listing-level data from the Hikari darknet archive—obtained
through direct academic collaboration with Nicolas Christin (Carnegie
Mellon University) and David Décary-Hétu (Université de Montréal)—to
study bilateral trade flows, enforcement structure, and spatial patterns
in illicit markets.

I work primarily in **Stata and R**, with an emphasis on large-scale data
cleaning, classification pipelines, and high-dimensional econometric
estimation.

---

## Working Paper

**Digital Illicit Trade and the Geography of Retail Drug Markets:  
Evidence from Cryptomarkets Using a Gravity Framework**  
*Working Paper, April 2026*

Using 354,000+ listing-level observations from 10 darknet cryptomarkets
collapsed to a bilateral country-pair × drug-type × month panel, I
estimate PPML gravity models with high-dimensional fixed effects.

**Core findings:**
- Distance elasticity ≈ **−2.05**
- Contiguity, common language, and colonial ties carry **large negative coefficients**  
  (inverse of all standard licit-goods gravity results)
- Effects operate entirely through the **intensive margin**
- Results are consistent with **bilateral enforcement coordination suppressing trade**
  on jurisdictionally familiar corridors

SSRN: *(link pending)*  
Replication code: https://github.com/rydermawby/darknet-gravity-model

---

## Data & Methods

- **354,212 cleaned observations** across 10 cryptomarkets (2014–2022)
- **50+ exporting countries**, **90+ importing countries**
- Hikari darknet archive (via Nicolas Christin, CMU)
- Supplementary archive (via David Décary-Hétu, Université de Montréal)
- CEPII Gravity Database (distance, language, contiguity, colonial ties)

### Classification Pipeline
- 8-stage multilingual keyword matching system
- 57 granular drug categories across 5 languages
- Collapsed to agricultural vs. synthetic for main analysis

### Estimation Framework
- Poisson Pseudo-Maximum Likelihood (**ppmlhdfe**)
- High-dimensional fixed effects (exporter-time, importer-time, pair FE)
- Extensive vs. intensive margin decomposition

---

## Repository Contents

| File | Description |
|------|-------------|
| `gravity_pipeline_v16.do` | Full gravity estimation pipeline |
| `MASTER_PIPELINE.do` | Drug classification pipeline |
| `Mawby_Drug_Appendix_MASTER.xlsx` | Drug taxonomy (57 categories) |

---

## Data Availability

Raw data are not included due to size and data-sharing agreements.

Access may be available for replication purposes upon request, subject
to original provider constraints.

---

## Research Direction

Ongoing work focuses on:
- Expanding bilateral coverage using the full Hikari archive (21 markets)
- Identifying synthetic vs. agricultural distance differentials
- Directly measuring enforcement coordination (MLATs, joint operations)
- Linking platform trade to offline trafficking structures

---

## Acknowledgments

Data and guidance provided by:

- Nicolas Christin (Carnegie Mellon University)
- David Décary-Hétu (Université de Montréal)

---

## License

Code is provided for academic and research use.  
Please cite the working paper if using the classification pipeline or
empirical framework.
