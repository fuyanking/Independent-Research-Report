# Public Perception of "Soul" in AI‑Generated Art: An Empirical Study Based on Multiple Linear Regression
Independent Research Project | Quantitative Social‑Science Research

## Project Overview
As generative AI techniques including GAN and Diffusion models gain popularity in artistic creation, there is ongoing public debate over whether AI‑generated artwork can possess a "soul". This independent research investigates factors that shape public perception of soul‑like qualities within AI art.

I collected 59 valid responses through an anonymous online questionnaire. This study applies **Cronbach’s α reliability test**, **KMO‑Bartlett sphericity validity test**, ordinary least‑squares (OLS) multiple linear regression, and comprehensive regression diagnostics. Six independent variables are examined:
1. Identification with traditional artistic viewpoints
2. Self‑reported understanding of AI‑generation technology
3. Frequency of emotional responses triggered by AI artwork
4. Acceptance of AI as an artistic creation tool
5. Individual art‑exposure background
6. Gender (binary dummy variable)

The overall regression model is statistically significant ($F=11.18$, $p<0.001$), with adjusted $R^2 = 0.513$. This indicates the selected predictors jointly explain 51.3 % of the variance in public soul‑perception scores.

Key findings:
- 61.0 % of respondents tend to believe AI‑generated art can have a soul; 28.8 % hold negative views, and 10.2 % remain neutral.
- **Identification with traditional art views and gender are statistically significant predictors ($p<0.05$)**. Higher agreement with traditional art viewpoints correlates with higher perceived soulfulness of AI art. Male participants are more likely to perceive soul‑like qualities in AI art.
- AI technical knowledge, frequency of emotional responses, acceptance of AI as a creative tool, and personal art background show no statistically significant effects within this model.

## Repository Structure
```
├── README.md                     # English project overview
├── Independent Research Final Report(Chinese ver).pdf    # Full original research paper (Chinese version)
└── Independent Research Final Report(English ver).pdf    # Full translated research paper (English version)
```
 
## Research Pipeline
1. **Literature Review**: Reviewed existing scholarship on computational creativity, AI‑art reception, and public aesthetic judgment. Identified research gaps including limited multivariate regression work and the under‑studied variable of AI‑tool acceptance.
2. **Model & Hypothesis Construction**: Established a multi‑dimensional “cognition‑emotion‑tool‑demography” framework. The multiple‑linear‑regression model specification:

$$
Y=\beta_{0}+\beta_1X_1+\beta_2X_2+\beta_3X_3+\beta_4X_4+\beta_5X_5+\beta_6X_6+\epsilon
$$

3. **Data Collection**: Distributed anonymous online surveys and obtained 59 valid samples via non‑probability sampling. Latent variables were measured using 1‑5 Likert‑scale survey items.
4. **Data Cleaning & Reliability‑Validity Check**: Calculated Cronbach’s α for each survey dimension. One reverse‑worded item (Q19) was removed for poor internal consistency. KMO‑Bartlett test passed ($KMO=0.909$, $p<0.001$).
5. **OLS Regression**: Fitted the full linear model using Python `statsmodels`.
6. **Regression Diagnostics**: Evaluated multicollinearity via Variance Inflation Factor (VIF); tested residual normality with histograms and Q‑Q plots; inspected heteroskedasticity using residual‑versus‑fitted scatter plots. No major model‑assumption violations were found.
7. **Result Interpretation**: Interpreted regression coefficients, discussed practical suggestions, acknowledged study limitations, and proposed directions for future research.

## Study Limitations

- Limited sample size (\(N=59\)) and non‑probability sampling restrict population‑level generalizability.
- Questionnaire wording imperfections; reverse‑coded questions introduced potential respondent confusion.
- Observational regression captures correlation rather than definitive causal relationships.

## Future Research Directions

- Expand sample size and diversify participant demographics such as age, education, and geographic background.
- Combine quantitative survey results with qualitative interview evidence.
- Incorporate additional predictors such as artwork genre to enrich the regression model.

## References

Full bibliographic references are documented inside both attached PDF papers, including publications by Boden, Floridi, Millet, Pelowski and other scholars in experimental aesthetics and computational creativity.