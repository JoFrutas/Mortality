# Mortality
This code was developed to find and compare mortality in ICU setting in people below and above 81 yars old ading necessary libraries and setting up the R Markdown environment for documentation. The data, presumably stored in a CSV file, is read into R using read_csv() from the readr package. The dataset is then split into two groups based on age using the subset() function.

Further data processing includes renaming column names to adhere to a consistent format and removing rows with missing values using na.omit(). The class and structure of the data object are checked to ensure compatibility with subsequent analysis steps.

After ensuring the data's suitability, logistic regression models are fitted separately for groups above and below the age of 81 using the glm() function. Model coefficients, standard errors, z-scores, and p-values are calculated and compared between the two groups to identify significant differences.

Additionally, a decision tree model is built for each age group using the rpart() function with specified control parameters for cost-complexity pruning. Summary statistics for each decision tree model, including variable importance, are presented.
