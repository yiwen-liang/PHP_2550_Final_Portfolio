### Project 2: Regression Analysis

### Developing a Prediction Model For Composite Outcome of Tracheotomy and Death

This is the 2nd project assignment of PHP2550 Practical Data Analysis course at Brown University (Fall 23).

${\color{gray}Posted: 12/15/2023}$

#### Abstract

Bronchopulmonary dysplasia (BPD) is a chronic pulmonary condition characterized by inflammatory processes and lung scarring. Given the merits and drawbacks of tracheostomy placement, it becomes crucial to determine the criteria for tracheotomy and the optimal timing for referring a patient for this procedure. This project construct two prediction models for composite outcome of tracheotomy and death for infants with severe bronchopulmonary dysplasia at 36 weeks and 44 weeks. For both week-36 and week-44 models, we first use *lasso* and *best subset* for variable selection of fixed effects, then fit a mixed effects model using the fixed effects obtained through variable selection, incorporating random intercept for each center. The performances of these models will be evaluated using metrics including the Brier score, AUC, sensitivity, and specificity. The week-36 models have Brier scores around 0.07, and the week-44 models have Brier scores of approximately 0.06. All four models have AUC greater than 0.9 and threshold lower than 0.15. However, the calibration of all models are not ideal. The models constructed with all available variables up to 44 weeks were deemed more effective. These models provide clinicians with valuable tools for early prognosis, facilitating informed discussions with the families of infants at risk.

#### Guidelines

* *Project2_Updated.pdf*: the updated report of this project assignment after first submission and receiving feedback.

* *Project2_Updated.Rmd*: the updated code file (.rmd) for this report, including all codes for creating tables and figures in the report.

* *PHP2550_Project2_Yiwen_Liang.pdf*: the initial report of this project assignment.

* *PHP2550_Project2_Yiwen_Liang.Rmd*: the initial code file (.rmd) for this report, including all codes for creating tables and figures in the report.

#### Data Availability

The dataset used in this project is not available to the public.

#### Acknowledgement

This project is the collaboration with Dr. Christopher Schmid in the Department of Biostatistics, School of Public Health, Brown University, and the instructor is Dr. Alice Paul from Department of Biostatistics, School of Public Health, Brown University.
 
#### Environment Version Information

All analyses are performed in R v4.2.2, and the packages utilized in this project are listed below.

| Packages  | Version |
| ------------- | ------------- |
| `cowplot`  | 1.1.1   |
| `ggplot2`  | 3.4.3  |
| `ggpubr`  | 0.5.0  |
| `kableExtra`  | 1.3.4  |
| `knitr`  | 1.39  |
| `mice`  | 3.16.0  |
| `reshape2`  | 1.4.4  |
| `tidyverse` | 1.3.2  |

#### Authors

Yiwen Liang (yiwen_liang@brown.edu)

