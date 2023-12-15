### Project 3: Simulation Studies

### Evaluating the Performance of a Prediction Model in Different Population

This is the 3rd project assignment of PHP2550 Practical Data Analysis course at Brown University (Fall 23).

${\color{gray}Posted: 12/15/2023}$

#### Abstract

Evaluating the transportability of prediction models becomes crucial when considering their application in diverse target populations. Various methods have emerged to assess model performance in different populations, and this project focuses on transporting a cardiovascular disease (CVD) events model developed using Framingham Heart Study data to the broader National Health and Nutrition Examination Survey (NHANES) data in 2017. Three evaluations are conducted to gauge the model's performance in different scenarios. Firstly, in the original population of the Framingham study where the model is developed, Brier scores can be easily computed. Secondly, considering transporting the model to a new target population where individual-level data is accessible whereas the outcome is lacking, an alternative Brier score estimator proposed by Dr. Jon Steingrimsson is employed to assess the model's performance. Lastly, when only summary statistics of the target population are available, a simulated target population is created based on these statistics, and the estimated Brier score is utilized to assess the model's performance in the simulated population. The Brier scores and estimates from these evaluations are scrutinized to ascertain the model's accuracy and transportability. The Brier score is 0.1992 for men and 0.1118 for women within Framingham, and the averaging estiamted Brier score is 0.1323 for men and 0.0670 for women in NHANES. The Brier score from the simulation study have the mean of 0.1439 for men and the mean of 0.0573 with the standard deviation for women, which are close to the estiamted Brier scores using the origianl target population with individual-level data. Results indicate that the prediction model exhibits reasonable accuracy for CVD risk prediction, with better performance in females. Strong performance in simulation studies indicates substantial transportability of the cardiovascular disease events model from Framingham Heart Study data to the extensive NHANES data. Additionally, if the simulation of the target population is appropriately conducted, it's applicable for scientists to apply transportability analysis to a simulated data when the full data is not available. 

#### Guidelines

* *Project3_Updated.pdf*: the updated report of this project assignment after first submission and receiving feedback.

* *Project3_Updated.Rmd*: the updated code file (.rmd) for this report, including all codes for creating tables and figures in the report.

* *brier_est1.RDS*: the simulation results using uniform(1,75) to simualte `AGE`.

* *brier_est2.RDS*: the simulation results using beta(10,19)*100 to simualte `AGE`.

* *brier_est3.RDS*: the simulation results using truncated normal distribution, with lower bound = 1, and upper bound = 75 to simualte `AGE`.

* *brier_est4.RDS*: the simulation results using multivariate normal distribution.

* *PHP2550_Project3_Yiwen_Liang.pdf*: the initial report of this project assignment.

* *PHP2550_Project3_Yiwen_Liang.Rmd*: the initial code file (.rmd) for this report, including all codes for creating tables and figures in the report.

* *project3.R*: the code provided for pre-processing both datasets and constructing the mdoel for evaluation.

#### Data Availability

The data sources used in this project include data from `Framingham` and `NHANES` in 2017, and both are publicly available.

#### Acknowledgement

This project is the collaboration with Dr. Jon Steingrimsson in the Department of Biostatistics, School of Public Health, Brown University, and the instructor is Dr. Alice Paul from Department of Biostatistics, School of Public Health, Brown University.
 
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
| `nhanesA`  | 0.7.4  |
| `reshape2`  | 1.4.4  |
| `riskCommunicator`  | 1.0.1  |
| `tableone`  | 0.13.2   |
| `tidyverse` | 1.3.2  |
| `truncnorm` | 1.0-9  |

#### Authors

Yiwen Liang (yiwen_liang@brown.edu)

