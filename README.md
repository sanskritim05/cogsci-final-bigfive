# Big Five Personality Traits Across the Lifespan

## Overview
This project explores how the Big Five personality traits (Extraversion, Agreeableness, Conscientiousness, Neuroticism, and Openness) change across age. Using a large publicly available dataset, the project examines personality patterns from adolescence through older adulthood. The goal is to clearly communicate how personality develops over the lifespan using accessible explanations and visualizations.

This repository includes data cleaning, trait scoring, exploratory analysis, and a final science communication document created in Quarto.

## Data Source
The data comes from an online Big Five personality test hosted by OpenPsychometrics and collected around 2012. Participants completed a 50-item personality questionnaire using a 1–5 Likert scale (1 = Disagree, 5 = Agree). Each of the Big Five traits is measured using 10 items.

In the raw dataset, a response value of `0` indicates that the participant skipped a question. These values were treated as missing (`NA`) during data cleaning. Demographic information, including age, was used to examine how personality traits change across the lifespan.

This project is a secondary data analysis; no new data was collected by the author.

## Project Structure
- **Exploratory analysis notebook**: exploratory_big5.Rmd, exploratory_big5.nb.html
  - A Quarto/HTML notebook used for data cleaning, reverse scoring of negatively keyed items, computation of trait scores, descriptive statistics, and exploratory visualizations.

- **Science communication document**: infographic_big5.qmd, infographic_big5.html
  - A camera-ready Quarto document designed for a general audience. This file presents the results without displaying any R code and focuses on interpretation and insight. Interactive plots allow readers to explore personality trends across age.

## Methods
Skipped responses were converted to missing values and negatively keyed items were reverse scored so that higher values consistently reflect higher levels of each trait. Trait scores were computed by averaging the relevant items for each participant.

The analysis focuses on participants aged 13 to 90. Smoothed trend lines were used in the visualizations to highlight long-term age-related patterns rather than short-term variation.

## Intended Audience
This project is intended for intelligent non-experts, such as students or readers interested in psychology who may not have a background in statistics or data analysis. The explanations and visualizations are designed to be clear and readable.

## Key Insight
The findings suggest that personality traits are not fixed over time. Some traits tend to increase with age, while others show more gradual or complex changes. Overall, the results support the idea that personality continues to develop throughout the lifespan.

## Tools Used
- R  
- Quarto  
- tidyverse  
- ggplot2  

## Author
**Sanskriti Malakar**  
