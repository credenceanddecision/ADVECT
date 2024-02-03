# ImpactATTAnalyzer
ImpactATTAnalyzer facilitates the estimation of Average Treatment Effect on the Treated (ATT) using the Conditional Independence Assumption (CIA), tailored for marketing campaign data.

## Example scenario

A national wine merchant aims to enhance wine club memberships by encouraging households to purchase a minimum of 12 bottles via a targeted advertising campaign. The "ImpactATTAnalyzer" tool is utilized to design and evaluate this campaign, focusing on identifying households most likely to respond based on variables like wine consumption level, purchase history, and preferences. By conducting power analysis and estimating the Average Treatment Effect on the Treated (ATT) using the Conditional Independence Assumption (CIA), the merchant can efficiently allocate resources, target the campaign more effectively, and measure its impact, optimizing marketing strategies for increased engagement and sales.

## Usage

After installing the necessary libraries, execute the Jupyter notebook `ImpactATTAnalyzer.ipynb`:

1. Conduct a power analysis to determine the necessary sample size for reliable results.
2. Preprocess the data to fit the model's requirements.
3. Estimate the ATT by comparing the premium wine interest of households exposed to the advertising campaign against those not exposed, while controlling for confounding variables.

## Data Description

The dataset includes the following key metrics:

- `ad_exposure_wine_club`: Indicator if a household was exposed to the wine club ad campaign.
- `wine_club_signup`: Indicator if the household signed up for the wine club post-exposure.
- `digital_engagement_level`: Engagement with online wine-related content.
- `household_wine_spending`: Annual spending on wine, indicative of purchasing power.
- `wine_preference_diversity`: Diversity of wine preferences, potentially indicating openness to wine club offerings.
- `previous_wine_purchase_online`: Indicator of readiness to buy wine through the wine club.
- `premium_wine_interest`: Interest in premium wine consumption.

## Results Interpretation

The tool provides various output forms to interpret the campaign's effectiveness:

- T-tests to assess the significance of differences in observable characteristics between treated and untreated groups.
- Propensity score matching to estimate ATT.
- Visualization aids such as histograms and scatter plots to assess the propensity score distribution and the covariate balance after matching.

