# Seabird Avoidance Rates
Code and data to calculate seabird avoidance rates for collision risk modelling. This uses data from observed collisons from numerous onshore windfarms and the Thanet offshore wind farm. This work built on the avoidacne rates calculated in [Cook (2021)](https://www.bto.org/sites/default/files/publications/bto_rr_739_cook_collision_risk_models_final_web.pdf)

## Authors
- Luke Ozsanlav-Harris
- Richard Inger
- Richard Sherley

## Code description
- `Ozsanlav-Harris et al (2022) markdown code.rmd` Markdown file to calcualte avoidance rates using four different models:
  - Basic Band
  - Extended Band
  - Stochastic Basic Band
  - Stochastic Extended Band

## Data description 
- `Ozsanlav-Harris et al (2022) Collision Data.csv` main data file containing the number of collisions, correction factors, pasage rates and monitoring periods for each study included in the analysis
- `Flight Height Data.csv` proportion of birds flying at various heights for a given species. Each row in that data set represents the proportion of birds flying within a 1m interval. I.e. row 54 gives the proportion of birds for a given species flying between 53m and 54m.
- `BH_Boot.csv` Black-headed Gull bootstrapped flight heights
- `CG_Boot.csv` Common Gull bootstrapped flight heights
- `CT_Boot.csv` Common Tern bootstrapped flight heights
- `GB_Boot.csv` Great Black-backed Gull bootstrapped flight heights
- `HG_Boot.csv` Herring Gull bootstrapped flight heights
- `KI_Boot.csv` Kittiwake bootstrapped flight heights
- `LB_Boot.csv` Lesser Black-backed Gull bootstrapped flight heights
- `LG_Boot.csv` Little Gull bootstrapped flight heights
- `NE_Boot.csv` Sandwich Tern bootstrapped flight heights

## Output description
- `SuggestedARs/BasicBandAR_ table.png` Basic Band avoidance rates 
- `SuggestedARs/StBasicBandAR_ table.png` Stochastic basic Band avoidance rates
