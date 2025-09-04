# Heart_disease_risk_analysis

### Project Overview
This project is a data analysis of the Framingham Heart Study using Python. This project aims to explore the Risk Factors for patients having a risk of Coronary Heart Disease (CHD) within the next 10 years.

### Data Sources
The primary data set used for this analysis is the framingham_heart_study.csv file, containing detailed information about each patient either at risk or not at risk of heart disease. This is a data set containing a list of 4,240 patients belonging to one of two categories: Either at risk of CHD or not at risk of CHD. This data set can be downloaded from the following website   (https://www.kaggle.com/datasets/noeyislearning/framingham-heart-study)

### Tools Used 
The tools used in this project are the main data analysis libraries of Python. These include:
•	Pandas
•	Matplotlib
•	Seaborn
•	SciPy


### Data Preperation 
In the initial data preperation phase, the following tasks were performed:
1. Data loading and inspection 
2. Data formatting 
3. Handling missing values

### Exploratory data analysis
EDA involved exploring the heart study data to answer key questions such as: 
- Do at-risk patients tend to have higher average BMI, systolic BP, cholesterol, and heart rate? 
- Do older people tend to be at a higher risk of heart disease compared with younger people. If so, why? 
- Do a higher % of people who are at risk of heart disease tend to be smokers? 
- Do a higher % of people who are at risk of heart disease tend to have a history of hypertension? 
- For smokers only, is there a correlation between number of cigarettes smoked per day and people’s ages. Do older people tend to smoke a higher number of cigarettes?
- Which numerical health metric features tend to have the strongest correlation with each other?

### Data Analysis 
Please see the python file for the code used in this project

### Results/Findings 
The following findings are obtained from the analysis:
1. Yes, most at risk patients do have a higher average BMI, systolic BP, cholesterol and heart rate.
2. A one-tailed Welch’s t test is performed on the data to determine if the mean cholesterol level, glucose level, BMI, Heart rate, Systolic BP and Diastolic BP of at-risk patients is significantly higher than for not-at-risk patients. The results of the test clearly indicate that this is the case. 
Assuming a significance level of α = 0.01, 
The p-values for the total cholesterol level, glucose level, Heart Rate, Systolic BP and Diastolic BP are less than 0.01 (p < 0.01) therefore the differences are statistically significant. This indicates that the higher values of the total cholesterol level, glucose level, Heart Rate, Systolic BP and Diastolic BP for at-risk patients are unlikely to be due to chance.
The only health feature which is an exception to this is the BMI. There is not enough statistical evidence to suggest that at risk patients have a significantly higher BMI than not-at-risk patients. 
3. The distribution of people’s ages is random. A high frequency of old and middle-aged people is at risk of heart disease. 
The histogram has three separate peaks and so has a multimodal distribution. 
These peaks suggest there may be three subgroups of at-risk individuals with different age ranges.
This suggests multiple subgroups within the at-risk population that are more likely to develop heart disease at different ages — possibly due to:
a)	Different lifestyle or genetic risk factors
b)	Underlying clusters or demographics
4. About the same % of people who are at risk of heart disease tend to be smokers as the % of people who are not at risk of heart disease. About 52 % of at-risk patients are smokers while 48% are non-smokers. About the same figure - 49% of not-at-risk patients are smokers while the remaining 51% were non-smokers. 
Hypertension refers to high blood pressure. 
5. A higher % of people who are at risk of heart disease tend to have a history of hypertension. About 50% of the patients at risk of heart disease do have a history of hypertension. On the other hand, only 27% of the patients not at risk of heart disease have a history of hypertension. So clearly a much higher % of at-risk patients have a history of hypertension than the patients belonging to the ‘not at risk’ category. 
6. For patients who are smokers only, there does not seem to be any correlation between people’s ages and the number of cigarettes per day. The two variables are independent of each other.

### Recommendations
- Instead of just looking at charts and graphs, more advanced statistical methods could be applied on the data to better understand how different health factors are connected. This would verify whether patterns we see in the visuals are actually meaningful or just random.
- The results from this analysis could be used to create clear, easy-to-understand messages for the public to offer health advice. For example, showing how smoking or high blood pressure increases the risk of heart disease could help raise awareness and encourage healthier choices.


### Limitations
While this project does provide useful findings from the Framingham Heart Study dataset, several limitations should be acknowledged:

1. The dataset primarily represents a white, middle-class population from Framingham, Massachusetts. Therefore, these findings and results might not be generalizable to more diverse ethnic and socioeconomic groups.
2. Several records contain missing values for key health metrics (e.g., cholesterol, BMI, smoking status). Although imputation techniques were applied, they may introduce bias or reduce model reliability.
3. Only 15 attributes of patients are included ignoring potentially influential factors such as stress level, diet and physical activity.
4. Some features, like smoking status, are reported by the patients themselves and so may be subject to individual bias.
5. Treating coronary heart disease as a simple yes/no outcome may overlook the gradual and complex nature of cardiovascular heart disease risk, which typically develops over time and varies in severity.











