# Seabird Avoidance Rates for Collisison Risk Modelling 🦅🎏

## Summary 📊
Code and data to calculate seabird avoidance rates for collision risk modelling. This uses data on direct bird collisions and passage rates from numerous onshore windfarms and the Thanet offshore wind farm to calculate a value for meso and micro-scale avoidance combined. This work builds on the avoidance rates calculated in [Cook (2021)](https://www.bto.org/sites/default/files/publications/bto_rr_739_cook_collision_risk_models_final_web.pdf) and updates the recommended avoidance rates for the UK seabirds. The avoidance rates we recommend are located in the folder `SuggestedARs/` but note that these will differ slightly from those generated by running the analysis with the code and data provided here since data from a single windfarm was removed due to data permissions.

## Authors 🖊️
- Luke Ozsanlav-Harris <a itemprop="sameAs" content="https://orcid.org/0000-0003-3889-6722" href="https://orcid.org/0000-0003-3889-6722" target="orcid.widget" rel="noopener" style="vertical-align:top;"><img src="https://orcid.org/sites/default/files/images/orcid_16x16.png" alt="ORCID iD icon" target="_blank" style="width:1em;margin-right:.5em;"/></a>
- Richard Inger <a itemprop="sameAs" content="https://orcid.org/0000-0003-1660-3706" href="https://orcid.org/0000-0003-1660-3706" target="orcid.widget" rel="noopener" style="vertical-align:top;"><img src="https://orcid.org/sites/default/files/images/orcid_16x16.png" alt="ORCID iD icon" target="_blank" style="width:1em;margin-right:.5em;"/></a>
- Richard Sherley

## Link to report 🔗
The final published report can be found at the follwing link: [https://hub.jncc.gov.uk/assets/de5903fe-81c5-4a37-a5bc-387cf704924d](https://hub.jncc.gov.uk/assets/de5903fe-81c5-4a37-a5bc-387cf704924d)

**NOTE**: there was a follow up report that re-calculated avoidance rates using a slightly altered method. This was lead by Stephen Lang and can be found here: [https://data.jncc.gov.uk/data/de5903fe-81c5-4a37-a5bc-387cf704924d/jncc-report-732-annex-4-follow-on-analysis.pdf](https://data.jncc.gov.uk/data/de5903fe-81c5-4a37-a5bc-387cf704924d/jncc-report-732-annex-4-follow-on-analysis.pdf)

## Citation
Ozsanlav-Harris, L., Inger, R. & Sherley, R. 2023. Review of data used to calculate avoidance rates for collision risk modelling of seabirds. JNCC Report 732, JNCC, Peterborough, ISSN 0963-8091.

## Code description
- `Ozsanlav-Harris et al (2022) markdown code.rmd` Markdown file to calculate avoidance rates using four different collisions risk models; Basic Band, Extended Band, Stochastic Basic Band and Stochastic Extended Band

## Data description 
- `Ozsanlav-Harris et al (2022) Collision Data.csv` main data file containing the number of collisions, correction factors, pasage rates and monitoring periods for each windfarm included in the analysis
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
- `SuggestedARs/BasicBandAR_ table.png` Reccomended basic Band avoidance rates 
- `SuggestedARs/StBasicBandAR_ table.png` Reccomended stochastic basic Band avoidance rates
