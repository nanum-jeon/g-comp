# G-Methods Tutorial Series
Comprehensive introduction to causal inference using g-methods in R. Covers **G-formula** and **Marginal Structural Models (MSM)** for handling time-varying confounders.

## Tutorial Overview
| Tutorial | Focus | Method | Level |
|----------|-------|--------|-------|
| **01** | [Introduction to G-Computation](01_g_comp_intro.Rmd) | G-computation | 🟢 Beginner |
| **02** | [Linear vs. ML Models](02_g_comp_linear-vs-ml.Rmd) | G-computation | 🟡 Intermediate |
| **03** | [Heterogeneous Treatment Effects](03_g_comp_hte.Rmd) | G-computation | 🟡 Intermediate |
| **04** | [Time-varying Confounders](04_g_comp_intro_time_varying.Rmd) | G-computation | 🟡 Intermediate |
| **05** | [Marginal Structural Models](05_msm_time-varying.Rmd) | Inverse Probability Weighting | 🟡 Intermediate |

## Learning Paths
- **Beginners:** 01 → 02
- **Complete series:** 01 → 02 → 03 → 04 → 05
- **Method comparison:** 04 vs 05

## What You'll Learn
**Core concepts:** Why standard regression fails with time-varying confounders, g-methods (G-formula and MSM/IPW), parametric vs nonparametric approaches, model selection

**Practical skills:** G-computation implementation, model validation, linear vs ML comparison, marginal structural models

## Prerequisites
- **R:** Intermediate level
- **Statistics:** Regression, basic probability
- **Causal inference:** Not required

## Tutorial Details
**01: Introduction** - Master basic g-computation with nonparametric and parametric g-formula

**02: Linear vs. ML** - Choose appropriate models comparing linear regression vs machine learning

**03: Heterogeneous Treatment Effects** - Estimate treatment effect heterogeneity using g-computation

**04: Time-varying Confounders** - Handle temporal confounding with sequential g-computation

**05: Marginal Structural Models** - Alternative approach using inverse probability weighting

## Dataset
Simulated HIV treatment data from [Naimi, Cole, and Kennedy (2017)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6074945/): HIV treatment over 2 periods with therapy regimen (A₀, A₁), time-varying viral load (Z₁), CD4 outcome (Y), and known true effect of 50.

## Quick Start
1. Download all `.Rmd` files
2. Start with Tutorial 01
3. Progress sequentially

## Citation
> Naimi, A. I., Cole, S. R., & Kennedy, E. H. (2017). An introduction to g methods. *International Journal of Epidemiology*, 46(2), 756-762.
