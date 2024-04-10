# Introduction

Insurance firms frequently struggle to calculate proper premiums for each policyholder in the health insurance market. Mistakes in evaluating health hazards can lead to large financial losses. Thus, in order to keep insurance businesses financially stable and give policyholders fair services, it is essential to determine health insurance premiums accurately. For this project, we will use a dataset that includes details about health insurance customers, such as their age, gender, BMI, number of children, smoking habits, home area, and specific medical bills that the insurance has billed. This dataset is a useful resource for building predictive models that help health insurance companies evaluate risks and establish more precise insurance rates. Additionally, greater risk assessment can help insurance companies create a range of products that better meets the demands of policyholders, increasing their competitiveness in the market. As a result, this project immediately affects the operations and business plans of health insurance providers, ultimately benefiting both the providers and their clients.

# Objective

This project's main goals are to create prediction models that can assist health insurance firms in the following areas:

1. **Precise Premium Determination**: By using policyholder data, premiums can be more precisely determined by taking into account the health risks that each policyholder faces. As a result, insurance companies can reduce the amount of money they lose because of incorrect premiums.
   
2. **Health Risk Assessment**: Determine risk factors, such as age, BMI, number of children, and smoking habits, that affect a person's medical expenses. This can aid insurance companies in better risk assessment and management.
   
3. **Product Portfolio Development**: Create insurance products that, depending on the features of each policyholder, more closely match their unique demands in order to increase customer satisfaction.

# Attribute Information

- **age**: Age of primary beneficiary
- **sex**: Insurance contractor gender, female, male
- **bmi**: Body mass index, providing an understanding of body, weights that are relatively high or low relative to height, objective index of body weight (kg / m2) using the ratio of height to weight, ideally 18.5 to 24.9
- **children**: Number of children covered by health insurance / Number of dependents
- **smoker**: Smoking
- **region**: The beneficiary's residential area in the US, northeast, southeast, southwest, northwest.

# Criteria Covered

1. **Data Cleaning**: Data cleaning involves rectifying or eliminating corrupted, improperly formatted incomplete data, within a dataset. When merging data sources there are possibilities for data duplication or mislabeling. As part of the data cleaning, we removed the rows that have null values in some columns. These null columns produce flawed visualizations and give erroneous results when worked upon for numerical or statistical computations.

2. **Linear Regression**: Linear regression is an analysis tool for estimating the value of one variable by considering the value of another variable. The variable that we want to estimate is known as the dependent variable while the variable we employ to predict its value is referred to as the independent variable. In this scenario, we have used linear regression techniques to predict values such as the yearly income or subscriber count if a new channel were to be started in a particular genre with a particular characteristic.

3. **Statistical Analysis**: Statistical analysis involves the gathering and interpretation of data to identify patterns and trends. It plays a role in data analytics aiding in research interpretation modeling, survey design and study implementation. In our case, we used statistical analysis to calculate the statistical values that play a crucial role in analysis or visualization.

# Code Analysis

- Loading the data
- Exploratory Data Analysis
- Multivariate analysis
- Hypothesis testing
- Correlation analysis
- Model Building - LINEAR REGRESSION

# Conclusion

Based on the analysis and modeling conducted, here are some key points that can be summarized:

- Through correlation analysis using Spearman and Pearson, as well as exploratory data analysis (EDA), we have identified that the feature with a significant influence on insurance bills is "smoker." Additionally, the features "age," "bmi," and "children" also have a notable impact on insurance bills.

- Based on the permutation feature importance analysis, it turns out that not only those four features have an impact on the model, but "region_northwest" and "region_northeast" also contribute to the model's performance. This phenomenon may occur due by several factors, notably the availability of higher-cost healthcare facilities compared to other regions, elevated risks associated with natural disasters, or stringent insurance regulations in comparison to other areas. However, the influence of "region_northwest" and "region_northeast" is relatively small but in this experiment, we have attained an improved score when compared to utilizing only four features.

- The Linear regression model has proven to be the best model in this experiment, primarily because it is more robust to outliers compared to Linear Regression.
