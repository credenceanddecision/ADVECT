# ADVECT
**ADVECT (ADVertising Effectiveness & Conditional Treatment Analyzer)** is designed to estimate the Average Treatment Effect on the Treated (ATT) using the Conditional Independence Assumption (CIA), specifically tailored for analyzing marketing campaign data.

## Example Scenario

A national wine merchant seeks to boost wine club memberships through a targeted advertising campaign, encouraging households to purchase a minimum of 12 bottles. ADVECT is employed to strategize and assess this campaign, pinpointing households with the highest likelihood of response based on wine consumption levels, purchase history, and preferences. Utilizing power analysis and the CIA to estimate ATT, the tool allows for efficient resource allocation, enhanced targeting, and impactful measurement of the campaign's success, ultimately optimizing marketing strategies for greater engagement and sales.

## Usage

To utilize ADVECT, follow these steps after installing the required libraries:

1. Run the Jupyter notebook `ADVECT.ipynb`:
    - Conduct a power analysis to determine the necessary sample size for robust results.
    - Preprocess the data according to the model's requirements.
    - Estimate the ATT by analyzing the interest in premium wine among households exposed to the advertising campaign versus those not exposed, controlling for confounding variables.

## Data Description

The dataset for ADVECT should include key metrics such as:

- `ad_exposure_wine_club`: Indicates whether a household was exposed to the wine club advertising campaign.
- `wine_club_signup`: Indicates whether the household signed up for the wine club following exposure.
- `digital_engagement_level`: Level of engagement with online wine-related content.
- `household_wine_spending`: Annual expenditure on wine, reflecting purchasing power.
- `wine_preference_diversity`: Variety in wine preferences, which may suggest openness to wine club offerings.
- `previous_wine_purchase_online`: Indicates prior online wine purchases, suggesting readiness to engage with the wine club.
- `premium_wine_interest`: Interest in premium wine varieties.

## Results Interpretation

ADVECT provides insights into the effectiveness of marketing campaigns through:

- T-tests to evaluate significant differences in characteristics between treated and control groups.
- Propensity score matching to accurately estimate the ATT, offering a deeper understanding of the campaign's impact on targeted households.
