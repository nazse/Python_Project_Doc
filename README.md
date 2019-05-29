
# **Project: The Basal Forebrain and CSF biomarkers data Model**

### *Data Source: The Gothenburg H70 Studies: 1944 Cohort examine in 2014*
###### *Author: Nazib M. Seidu*

#### **Overview: To do in Python ( Use: Jupyter-notebook)**
       Load Python Packages to workspace; Pandas, numpy, statsmodels.formula.api, seaborn, matplotlib and sklearn.preprocessing 
       Input file; CSV file (CSF_Python_update.csv)containing covariates, CSF biomarkers, Basal forebrain 
       Store in data frame (my_data_frame)
       View first few rows and columns ofthe data frame using head.()
       Check the dimension of the data frame to get an idea of number of observations and columns __.shape

#### **Descriptive Statistics: groupby.()**
       Group by Sex 
       Group by all the three CSF Pathological biomkers (ABeta, TTau and PTau)
       Group by Apoe4 Allele

#### **Visualations of data to for patterns (Correlation Matrix and Boxplots)**
       Convert binary variables to (0,1) unit for easy use; pd.get_dummies()
       Symmetric Correlation Matrix; __cor.()
       Boxplots for different combination of variables using library sns.()

#### **Gender Proportions with CSF Pathological changes and Apoe4 Risk Gene** 
       Amyloid pathology(pg/mL) and Gender proportions
       Total Tau pathology(pg/mL) and Gender proportions
       Phospho Tau pathology(pg/mL) and Gender proportions
       Apoe4 risk gene and Gender propoetions

#### **Format string inputs in data frame**
       Recode variables in string format to binary observation (0, 1); Where 0 = negative and 1 = positive
       Subset Response variables for our models
       Use For Loop and If esle statements ( ABeta, TTau and PTau) to exctract response variables in "CSF_target"

#### **Fitted Models: CSF Biomarkers Pathology and Basal Forebrain Models ; Logistic Regression Model - smf.logit()**
       We use For Loops, If, Elif and Else statements to iterate over dataset
       For each condition saity by the if statement we proceed and fit Model 1, Model 2 and Model 3 and excute with a pass in Else statement
       For each model, we fit same covariates store in formula as string for the three CSF biomarkers in CSF_target

#### **Print Command: Print important statistics for inferential purposes (Estiames, Z-Values, P-Values, OR, 95 % CI etc)**
       This loops continuous until we ouput our last CSF Pathological Model and loop ends

