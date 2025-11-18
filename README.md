# Fear-of-the-Supercompetitor

## Overview

This repository contains the data and code for analyzing white-tailed deer (*Odocoileus virginianus*) behavioral responses in auditory playback experiments. The analysis examines sex-specific responses across four behavioral metrics in response to coyote (*Canis latrans*) and wild pig (*Sus scrofa*) audio cues compared to a non-threatening control.

## Repository Structure
```
├── data/
│   ├── flight_model_data.csv
│   ├── vigilance_model_data.csv
│   ├── disturbance_model_data.csv
│   └── aggregate_feeding_model_data.csv
├── scripts/
│   └── ABR_Code.R
└── README.md
```

## Data Description

All datasets contain independent observations from playback experiments at baited foraging sites.

### Common Variables

- `Treatment`: Sound treatment (Control, Coyote, Pig)
- `sex`: Individual sex 
- `ABR_site`: Unique site identifier 

### flight_model_data.csv

**Response variable:** `fled` (binary: did individual flee from site after playback)

### vigilance_model_data.csv

**Response variable:** `vigilance_increased` (binary: did vigilance increase post-playback)

### disturbance_model_data.csv

**Response variable:** `individual_disturbed` (binary: was individual disturbed by playback)

### aggregate_feeding_model_data.csv

**Response variable:** `total_videos` (count: number of videos in which deer were detected 30-minutes after playback)

## Requirements

### R Version

R version >= 4.0.0

### R Packages
```r
library(lme4)         # Mixed-effects models
library(ggeffects)    # Model predictions
library(gridExtra)    # Plot arrangement
library(emmeans)      # Post-hoc comparisons
library(tidyverse)    # Data manipulation and visualization
```

## Reproducibility & Publishing

This repository is prepared to be published on Dryad alongside the associated manuscript. It contains all data and code needed to reproduce key results, following best practices for reproducible open science.


