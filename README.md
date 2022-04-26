# Workplace stress in real time: Three parsimonious scales for the experience sampling measurement of stressors and strain at work
The present repository includes the supplementary materials of the article "*Workplace stress in real time: Three parsimonious scales for the experience sampling measurement of stressors and strain at work*" by Luca Menghini, Massimiliano Pastore, and Cristian Balducci, accepted for publication in European Journal of Psychological Assessment (2022). Supplementary materials are also available at [this OSF repository](https://osf.io/87a9p/?view_only=8439d7578f54405a853b31264df9bc19), anonymized for peer-reveiw.

## Supplementary materials
- `S1_PowerAnalysis`: Riproducible R code&sup1; and generated [full report](https://Luca-Menghini.github.io/ESMmeasures-workplaceStress/S1_PowerAnalysis/S1_powerAnalysis_fullReport.html) of the a priori power analysis of the multilevel confirmatory factor analysis used to evaluate the factor structure of the three scales. A more synthetic PDF report is [depicted at this page](https://Luca-Menghini.github.io/ESMmeasures-workplaceStress/S1_PowerAnalysis/S1_powerAnalysis_shortReport.pdf).

- `S5_scopusSearch`: Results of the Scopus search of ESM studies on job stressors and strain (XLSX).

- `S3_ESMprotocol&scales`: Detailed description of the experience sampling methods (ESM) protocol used in the study, including the JSON protocol used with the [Sensus mobile application](https://predictive-technology-laboratory.github.io/sensus/), and the evaluated ESM scales (with Italian items and English translations). The PDF report describing the protocol and the evaluated ESM scales is [depicted at this page](https://Luca-Menghini.github.io/ESMmeasures-workplaceStress/S3_ESMprotocol%26scales/S3_ESMprotocol%26scales.pdf).

- `S4_dataAnalysis`: Riproducible R code&sup2; and generated [full report](https://Luca-Menghini.github.io/ESMmeasures-workplaceStress/S4_dataAnalysis/S4_dataAnalysis_fullReport.html) of the data pre-processing and data analysis procedures described in the article, also including a detailed report (PDF) of [multilevel confirmatory factor analysis](https://Luca-Menghini.github.io/ESMmeasures-workplaceStress/S4_dataAnalysis/S4.1_MCFAdetails.pdf), anad a [supplementary analysis of time trends, measurement reactivity, and sensitivity to contextual factors](https://Luca-Menghini.github.io/ESMmeasures-workplaceStress/https://github.com/Luca-Menghini/ESMmeasures-workplaceStress/blob/main/S4_dataAnalysis/S4.2_SensitivityToContextualFactors.pdf).

- `S5_rawData`: Raw CSV data used for running the data analysis script S4

### Notes
1. the first part of the `S1_powerAnalysis_code.Rmd` generates three datasets (`TDS_PARAMETERS.RData`, `TCS_PARAMETERS.RData`, and `MDMQ_PARAMETERS.RData`) necessary to execute the commmands of the second part, which were too large to be shared but can be generated with the first part of the script (otherwise obtained upon request to the first author).

2. the `S4_dataAnalysis_code.Rmd` script should be run from line 227. Indeed, the very first step of raw data reading (lines 220-224) are skipped (`eval = FALSE`) due to the large number of JSON raw data files exported from the Sensus Mobile application, and to the personal data included in those files (e.g., mobile device identification code). Moreover, it should be noted that several chunks of code concerning the analysis of influential cases (section 4.6, e.g., lines 3846-3854) are also set with `eval=FALSE`, meaning that they are not run when lunching the `Knit` command. This was done to save computational time. In order to lunch the full script, it is neccesary to set those chunks with `eval = TRUE`, and to create a subfolder named "heywood cases".
