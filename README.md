# Clinical-prediction-model-with-Framingham-data
To study clinical prediction, I used framingham data.
The purpose of sharing this code is to brush-up codes and to discuss analysis approach.
Please review and teach me something mistake or making better codes. 

## Contents
1. ["data-cleanup"](framingham_data-cleanup.Rmd) is Rmd file to overview data distribution, missing rates, and clean up data ready-to-analysis.
2. ["missing imputation"](framingham_missing-imputation.Rmd) is Rmd file. Firsty, I assessed missing ditrtibution and type of missing. Then, I imputate missing term with missForest in R package.
3. ["data analysis"](framingham_data-analysis.Rmd) is final Rmd file. I developed prediction models, evaluated the perfomance and validated it.
   I develop three regression model:
     - Simple model(only liner term) with Elastic Net
     - Simple model(only liner term) with Backwards stepwise -> Maximum likelihood estimation 
     - complex model(adding spline term and interaction term) with Backwards stepwise -> Maximum likelihood estimation 
