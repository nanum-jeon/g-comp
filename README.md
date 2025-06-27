# G-Methods Tutorial Series

A comprehensive introduction to causal inference using g-methods, implemented in R. This tutorial series covers the two major approaches for handling time-varying confounders: **G-formula** and **Marginal Structural Models (MSM)**.

## Tutorial Overview

| Tutorial | Focus | Method | Complexity |
|----------|-------|--------|------------|
| **01** | [G-Formula: Static Confounders](01_g-formula_intro_static-confounders.Rmd) | G-computation | 🟢 Beginner |
| **02** | [G-Formula: Time-Varying Confounders](02_g-formula_intro_time-varying-confounders.Rmd) | G-computation | 🟡 Intermediate |
| **03** | [G-Formula: Linear vs ML Models](03_g-formula_linear-vs-ml.Rmd) | G-computation | 🟡 Intermediate |
| **04** | [MSM: Time-Varying Confounders](04_g-formula_msm_time-varying.Rmd) | Inverse Probability Weighting | 🟡 Intermediate |

## Learning Path

**For beginners:** Start with Tutorial 01 → 02  
**For comprehensive coverage:** Complete all tutorials 01 → 02 → 03 → 04  
**For method comparison:** Focus on Tutorials 02 and 04

## What You'll Learn

### Core Concepts
- When and why standard regression fails with time-varying confounders
- Two major g-methods: G-formula and MSM/IPW
- Nonparametric vs parametric approaches
- Model selection considerations

### Practical Skills
- Implementing g-computation in R
- Fitting and validating causal models
- Comparing linear models vs machine learning approaches
- Calculating and interpreting marginal structural models

## Prerequisites

- **R Programming**: Intermediate level
- **Statistics**: Regression analysis, basic probability
- **Causal Inference**: Helpful but not required (concepts explained)

## Required R Packages

```r
install.packages(c("dplyr", "knitr", "kableExtra"))
```

## Tutorial Details

### Tutorial 01: G-Formula with Static Confounders
**Goal**: Master basic g-computation concepts  
**Methods**: Nonparametric and parametric g-formula  
**Key Learning**: Foundation of causal inference with g-methods

### Tutorial 02: G-Formula with Time-Varying Confounders  
**Goal**: Handle temporal confounding  
**Methods**: Sequential g-computation  
**Key Learning**: Why timing matters in causal inference

### Tutorial 03: G-Formula Model Comparison
**Goal**: Choose appropriate models for g-computation  
**Methods**: Linear regression vs machine learning  
**Key Learning**: Bias-variance tradeoffs in causal modeling

### Tutorial 04: Marginal Structural Models
**Goal**: Alternative approach to time-varying confounding  
**Methods**: Inverse probability weighting  
**Key Learning**: When to use MSM vs g-formula

## Dataset

All tutorials use simulated HIV treatment data from [Naimi, Cole, and Kennedy (2017)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6074945/):

- **Setting**: HIV treatment over 2 time periods
- **Treatment**: Therapy regimen (A₀, A₁)  
- **Confounder**: Time-varying viral load (Z₁)
- **Outcome**: CD4 count (Y)
- **True causal effect**: 50 (known from data generation)

## Quick Start

1. **Clone or download** all `.Rmd` files
2. **Install required packages** (see above)
3. **Start with Tutorial 01** to build foundations
4. **Progress sequentially** through the series

## Key Results

All properly implemented methods recover the true causal effect of 50:

- ✅ Nonparametric g-formula: 50.0
- ✅ Parametric g-formula: 50.0 (with correct specification)
- ✅ MSM/IPW: 50.0 (with proper weighting)

## Support

Each tutorial includes:
- Step-by-step explanations
- Complete R code with comments
- Model validation and diagnostics
- Comparison of methods

## Citation

Based on methodology from:
> Naimi, A. I., Cole, S. R., & Kennedy, E. H. (2017). An introduction to g methods. *International Journal of Epidemiology*, 46(2), 756-762.

---

**Happy learning!** These tutorials provide a complete foundation for applying g-methods in your own causal inference projects.
