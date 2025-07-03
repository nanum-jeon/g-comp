# G-Methods Tutorial Series
A comprehensive introduction to causal inference using g-methods, implemented in R. This tutorial series covers the two major approaches for handling time-varying confounders: **G-formula** and **Marginal Structural Models (MSM)**.

## Tutorial Overview
| Tutorial | Focus | Method | Complexity |
|----------|-------|--------|------------|
| **01** | [Introduction to G-Computation](01_g_comp_intro.Rmd) | G-computation | 🟢 Beginner |
| **02** | [G-Computation: Linear vs. ML Model](02_g_comp_linear-vs-ml.Rmd) | G-computation | 🟡 Intermediate |
| **03** | [G-Computation: Heterogeneous Treatment Effect Estimation](03_g_comp_hte.Rmd) | G-computation | 🟡 Intermediate |
| **04** | [G-Computation: Time-varying](04_g_comp_time-varying.Rmd) | G-Computation | 🟡 Intermediate |
| **05** | [MSM: Time-varying](05_msm_time-varying.Rmd) | Inverse Probability Weighting | 🟡 Intermediate |

## Learning Path
**For beginners:** Start with Tutorial 01 → 02  
**For comprehensive coverage:** Complete all tutorials 01 → 02 → 03 → 04 → 05  
**For method comparison:** Focus on Tutorials 04 and 05

## What You'll Learn
### Core Concepts
- When and why standard regression fails with time-varying confounders
- Two major g-methods: G-Computation and MSM/IPW
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


## Tutorial Details
### Tutorial 01: G-Formula with Static Confounders
**Goal**: Master basic g-computation concepts  
**Methods**: Nonparametric and parametric g-formula  

### Tutorial 02: G-Formula with Time-Varying Confounders  
**Goal**: Handle temporal confounding  
**Methods**: Sequential g-computation  

### Tutorial 03: G-Formula Model Comparison
**Goal**: Choose appropriate models for g-computation  
**Methods**: Linear regression vs machine learning  

### Tutorial 04: G-Computation with Time-Varying Confounders
**Goal**: Advanced g-computation techniques  
**Methods**: Sequential g-computation with complex confounding  

### Tutorial 05: Marginal Structural Models
**Goal**: Alternative approach to time-varying confounding  
**Methods**: Inverse probability weighting  

## Dataset
All tutorials use simulated HIV treatment data from [Naimi, Cole, and Kennedy (2017)](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6074945/):
- **Setting**: HIV treatment over 2 time periods
- **Treatment**: Therapy regimen (A₀, A₁)  
- **Confounder**: Time-varying viral load (Z₁)
- **Outcome**: CD4 count (Y)
- **True causal effect**: 50 (known from data generation)

## Quick Start
1. **Clone or download** all `.Rmd` files
3. **Start with Tutorial 01** to build foundations
4. **Progress sequentially** through the series


## Citation
Based on methodology from:
> Naimi, A. I., Cole, S. R., & Kennedy, E. H. (2017). An introduction to g methods. *International Journal of Epidemiology*, 46(2), 756-762.

---
**Happy learning!** These tutorials provide a complete foundation for applying g-methods in your own causal inference projects.
