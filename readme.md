# Nonparametric Bayesian Instrumental Variable Analysis: Evaluating Heterogeneous Effects of Coronary Arterial Access Site Strategies

# Author Contributions Checklist Form

## Data

### Abstract

PCI data from a state-mandated clinical registry coordinated by the Massachusetts Data Center (Mass-DAC) are used. The clinical registry data include all PCIs performed in all nonfederal acute care Massachusetts hospitals for patients at least 18 years of age, regardless of health insurance status. The registry data are populated by trained data managers at each hospital. The registry data are linked to the Massachusetts Acute Hospital Case-Mix billing data maintained by the Massachusetts Center for Health Information and Analysis to obtain additional post-discharge hospitalization information, such as subsequent admissions for PCI, bypass surgery, heart attack, etc. Information is linked using criteria based on combinations of treatment hospital, medical record number, admission or discharge date, and date of birth. Vital status is determined using the Massachusetts Registry of Vital Statistics as well as the National Death Index.



### Availability 

The data used in this paper are not publicly available because they contain sensitive information about patient’s medical history. They can, however, be accessed from the Massachusetts Department of Public Health through a formal application.





##Code

###Abstract

We have developed an MCMC sampler along with summary functions to fit the proposed model in R. Some parts of the sampler are coded using Rcpp. The code is also available as an R package in its beta version and can be installed from its GitHub repository.
the code.

### Description 

The R code to run the sampler along with supporting functions for summarizing posterior draws and running simulations are available in GitHub as two separate repositories. The R package ‘BayesIV’ is available in GitHub repository https://github.com/SamAdhikari/BayesIV_0.1 .
The simulation code to generate some of the results in the paper is available in a separate GitHub repository https://github.com/SamAdhikari/BayesIV_Simulations .

A .tar.gz file is also submitted as a supplemental material.

### Optional Information 
Supporting R packages: Rcpp, DPpackage, msm
Additional packages required for simulation: ivpack, MASS
To install .tar.gz version of the R-package: linux, unix or mac OS
To install R package from Github: Windows, linux, unix or mac OS


## Instructions for Use


### Reproducibility

Table 2 is to be reproduced. A script titled ‘runSimulations.R’ is included in the GitHub repository https://github.com/SamAdhikari/BayesIV_Simulations to generate simulated data, run multiple replications on the data, and summarize the simulation results. A README file, that describes each of these simulation steps in detail, is also included in the repository


Warning: this code will take days to run; especially for bigger sample size.

For n = 100, twenty thousand MCMC iterations for 1 replication will take about 3 hours in a macOS High Sierra with 2.7 GHz Intel Core i7, 16 GB processor. Users can parallelize the code for multiple replications with different sample sizes.

