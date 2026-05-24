# Boston Housing Price Analysis

**Multiple Linear Regression Theory Project**  

---

## Overview

Analysis of the classic Boston Housing dataset (Harrison & Rubinfeld, 1978) to identify
the strongest predictors of median home values across 506 Boston census tracts.

--

## Research Question

> How effectively can we predict median owner-occupied home values using 13 neighbourhood-level
> predictors, and which are most influential?

--

## Notebook Contents

| Section | Description |
|---|---|
| 0. Setup | Imports and plot configuration |
| 1. Data | Dataset loading and data dictionary |
| 2. EDA | Univariate distributions, bivariate plots, correlation heatmap |
| 3. Methodology | Base, Reduced 1, Reduced 2 OLS models; VIF; Cook's Distance; refined model |
| 4. Results | Coefficient table, CI plot, key interpretations |
| 5. Discussion | Actual vs. predicted, feature importance, limitations |

--

## Key Findings

- **LSTAT** (% lower-status population) and **RM** (rooms per dwelling) are the strongest predictors.
- **PTRATIO** and **NOX** highlight the capitalisation of school quality and air quality into prices.
- Removing influential observations (Cook's D threshold) raised Adj R² from ~0.73 to ~0.84.
- River-adjacent tracts (CHAS=1) carry a ~$1,400 premium; each extra room adds ~$5,000.

--

## Requirements

```
numpy
pandas
matplotlib
seaborn
scipy
statsmodels
```

Install with:
```bash
pip install numpy pandas matplotlib seaborn scipy statsmodels
```

--

## Data

The dataset is the original Boston Housing data from the U.S. Census Bureau, as used in:

> Harrison, D. & Rubinfeld, D.L. (1978). Hedonic housing prices and the demand for clean air.
> *Journal of Environmental Economics and Management*, 5(1), 81–102.

--

## Acknowledgements

Final project for STA 221: Multiple Regression Theory and Applications — Duke University.
Team: Ashley Park, Kevan Wang, Jennifer Lee, Oliver Lublin.
