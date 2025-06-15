# Explainable GeoAI and statistical analysis reveal complementary insights about disparities of 311 help requests during the 2022 Buffalo blizzard

### Overall description
The 2022 Buffalo blizzard was a catastrophic winter storm that struck Buffalo, New York in the week of Christmas in 2022. It claimed 47 lives and left much of the region stranded for the holiday week. In this disaster, the 311 call service was used by many residents to request help for issues due to the blizzard. This study examines these 311 help requests and their potential disparities across communities. Specifically, we aim to: (1) understand the spatial and temporal distributions of different types of 311 help requests; (2) identify the physical and social vulnerability factors, as well as human behavior factors, that are associated with the use of 311 calls. Methodologically, we leverage both explainable geospatial artificial intelligence (GeoAI) methods and statistical analysis to analyze 311 help requests and their associated factors. Our analysis shows significant spatial disparities in 311 help requests across communities. Results from explainable GeoAI and statistical analysis also reveal complementary insights on key factors associated with 311 help requests, such as historical 311 request behavior and percentage of minority population. These results could inform future disaster management decisions and help mitigate the negative impacts of winter storm disasters.

This repository contains processed 311 request data, along with physical and social vulnerability variables, as well as previous 311 request behavior variables, for performing six different statistical and machine learning models. These models include the Spatial Lag Model (SLM), Spatial Error Model (SEM), Geographically Weighted Regression (GWR), Support Vector Machine (SVM), Random Forest (RF), and Geographical Random Forest (GRF). For more details, please refer to our full paper:

<I>Zhou, R.Z., Hu, Y., Sun, K., Muldoon, R., Clark, S. and Joseph, K., 2025. Explainable GeoAI and statistical analysis reveal complementary insights about disparities of 311 help requests during the 2022 Buffalo blizzard. International Journal of Disaster Risk Reduction, p.105635.</I>  [[PDF]](https://ryan-zhenqi-zhou.github.io/Manuscript_BuffaloBlizzard311.pdf)

<br />

<p align="center">
<img align="center" src="Figures/Study Design.png" width="600" />
<br />
Figure 1. An overview of the study design. (a) RQ1; (b) RQ2.
</p>

### Repository organization

* Data: This folder is organized to include various data and model outputs for the analysis. The SHAP result/ directory contains SHapley Additive exPlanations (SHAP) results used for model interpretability, while the shp/ folder holds geospatial data for spatial visualization. The datasets 311_data_12_19_filtered.csv and 311_data_19_15_filtered.csv provide processed 311 request data for spatial and temporal analysis. The file modeling.csv is used for the initial statistical and machine learning model development, while modeling_grf.csv is tailored for Geographical Random Forest (GRF) modeling. modeling_tuning_grf.csv contains data for hyperparameter tuning of the GRF model, and modeling_tuning_grf_result.csv stores the results of that tuning process.
* Code: This folder contains scripts for analyzing and implementing six different statistical and machine learning models.

### Project dependencies
* Python 3.12.3
