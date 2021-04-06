# ESMvalidation-workplaceStress
The present repository includes the supplemental materials of the article "*Workplace stress in real time: Four parsimonious scales for the experience 
sampling measurement of stressors and strain at work*" by Luca Menghini, Massimiliano Pastore, and Cristian Balducci.

The following supplemental materials are included:
- **S1**: A priori power analysis results
- **S2**: Reproducible R code used for power analysis
- **S3**: Detailed description of the ESM protocol and the proposed ESM scales
- **S4**: Complete data analysis report (html file to be open with any browser)
- **S5**: Raw data to be used for running the S6 script
- **S6**: Rmarkdown script to generate the S4 report using the S5 raw data
- **S7**: Example figures of ESM scales sensitivity to contextual factors

Note: the **S6** script should be run from line 227. Indeed, the very first step of raw data reading (lines 220-224) was skipped due to the large number of raw data files exported from the Sensus Mobile application, and to the personal data included in those files (e.g., mobile device identification code).
Moreover, it should be noted that several chunks of code concerning influential analyses (section 4.6, e.g., lines 3846-3854) are set with eval=FALSE, meaning that they are not run when lunching the Knit command. This was done to save computational time. In order to lunch the full script, it is neccesary to set those chunks with eval=TRUE, and to create a subfolder named "heywood cases".
