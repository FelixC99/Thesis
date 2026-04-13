# Replication Code: Evaluating the Efficacy of Anti-Misinformation Interventions: An Analysis of Demographic Differences
## Master Thesis — Felix Clausen, Universität zu Köln, 2026

This repository contains the analysis code for the empirical part of my 
Master's thesis, which examines the effectiveness of three 
anti-misinformation interventions (accuracy nudges, source ratings, 
fact-check labels) on sharing intentions and their demographic differences
using a pooled experimental dataset.

---

## How to Reproduce

Run the scripts **in order**:

1. `00_download_data.Rmd` — downloads all raw datasets from OSF automatically
2. `01_data_preparation.Rmd` — cleans and merges datasets into the analytical sample
3. `02_descriptive.Rmd` — produces descriptive statistics
4. `03_main_analysis.Rmd` — runs all models and generates figures

> All data are downloaded automatically. No manual data setup is required.

For convenience, pre-rendered HTML versions of all scripts are included 
in this repository. These allow inspection of all code, results and 
figures without re-running the analysis.
---

## Required R Packages

tidyverse, lme4, lmerTest, broom.mixed, ggeffects, ggplot2,
modelsummary, multcomp, emmeans, performance, DHARMa, simr,
forcats, haven, patchwork, archive, pandoc

Install all at once:
install.packages(c("tidyverse", "lme4", "lmerTest", "broom.mixed",
  "ggeffects", "modelsummary", "multcomp", "emmeans", 
  "performance", "DHARMa", "simr", "haven", "patchwork", "archive", "pandoc"))

