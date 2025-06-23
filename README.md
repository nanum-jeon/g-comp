# Introduction to G-Computation for Causal Inference

This repository contains tutorials that demonstrate how to implement **g-computation** (the g-formula) for estimating causal effects in both **static** (cross-sectional) and **time-varying** (longitudinal) settings. These materials are based on the framework introduced in:

> Naimi, A. I., Cole, S. R., & Kennedy, E. H. (2017).  
> *An introduction to g methods.* International Journal of Epidemiology, 46(2), 756–762.  
> [https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6074945/](https://www.ncbi.nlm.nih.gov/pmc/articles/PMC6074945/)

---

## Contents

### `gformula_linear.Rmd`
- Implements the g-formula in a simple cross-sectional setup
- Demonstrates both:
  - **Non-parametric g-computation** (standardization)
  - **Parametric g-computation** (via regression models)
- Includes comparison with unadjusted and stratified estimates

### `gformula_ML.Rmd`
- **Machine Learning G-Formula Implementation**
- Compares traditional parametric approaches with flexible ML methods
- Demonstrates nuanced performance of Random Forest vs linear models:
  - **Simple linear relationships**: Linear models outperform RF (RF adds unnecessary variance)
  - **Complex non-linear relationships**: RF captures heterogeneous effects better but doesn't always improve marginal ATE estimates
- Includes:
  - Cross-validation performance comparison
  - Treatment effect heterogeneity visualization
  - Practical guidance on trade-offs between flexibility and bias/variance

### Time-varying (coming soon)
---

## Getting Started

To run the tutorials:

1. Clone the repository or download the `.Rmd` files
2. Open the files in RStudio
3. Run interactively or knit to HTML
 
