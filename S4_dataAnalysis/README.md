## Notes:

- The `S4_dataAnalysis_code.Rmd` script should be run from line 227. Indeed, the very first step of raw data reading (lines 220-224) are skipped (`eval = FALSE`) due to the large number of JSON raw data files exported from the Sensus Mobile application, and to the personal data included in those files (e.g., mobile device identification code). 
- Moreover, it should be noted that several chunks of code concerning the analysis of influential cases (section 4.6, e.g., lines 3846-3854) are also set with `eval = FALSE`, meaning that they are not run when lunching the `Knit` command. This was done to save computational time. In order to lunch the full script, it is neccesary to set those chunks with `eval = TRUE`, and to create a subfolder named "heywood cases".
