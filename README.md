# Data-Driven Insights for Predicting Vaccine Uptake
## Project overview
The "Data-Driven Insights for Predicting Vaccine Uptake" project focuses on understanding the factors that influence individuals' decisions to receive the H1N1 vaccine. Using a structured data science workflow, the project examines survey data to identify key predictors of vaccination behavior and develops predictive models to support public health strategies.
This study addresses the critical need to improve vaccine adoption rates by identifying barriers and enablers of vaccination. It highlights the role of healthcare accessibility, doctor recommendations, and public perceptions of vaccine effectiveness and risk. Insights gained from this analysis are intended to guide public health interventions, enhance educational outreach, and inform policy-making to promote equitable vaccine uptake.

## Business understanding 
Vaccination represents a pivotal public health breakthrough that has controlled numerous infectious diseases. However, rising vaccine skepticism and declining immunization rates threaten this progress, potentially triggering preventable disease outbreaks.
This research analyzes the National Flu Survey (NHFS 2009) to predict H1N1 vaccine uptake, offering insights into vaccination behavior. By examining historical immunization patterns, the study provides relevant context for understanding vaccine acceptance, especially significant during emerging pandemic scenarios like COVID-19.
The analysis bridges historical data with contemporary public health challenges, highlighting the ongoing importance of understanding factors that influence individual vaccination decisions.

## Project objectives 
1.Prediction: Build machine learning models to forecast individuals' likelihood of receiving the H1N1 vaccine using demographic, socio-economic, and attitudinal data.

2.Influential Factors Analysis: Identify key factors influencing H1N1 vaccine uptake, such as doctor recommendations, health insurance status, perceptions of vaccine effectiveness, and perceived risk of contracting H1N1.

3.Model Performance Evaluation: Compare the effectiveness of various machine learning algorithms, including Decision Tree Classifier and Logistic Regression, in accurately predicting H1N1 vaccination behavior.

4.Insights and Recommendations: Analyze the results of the predictive models to provide actionable insights for public health officials and policymakers aimed at improving vaccination rates.

## Data understanding
The dataset used in this project provides a comprehensive view of the factors influencing H1N1 vaccine uptake. It includes demographic information, health-related attributes, and perceptions about the vaccine's effectiveness and the risk of contracting H1N1.
Key variables include:
- Demographics: Age, gender, income level, education, and household composition.
- Health Attributes: Presence of health insurance, underlying health conditions, and regular interactions with healthcare providers.
- Perceptions and Opinions: Respondents' beliefs about vaccine effectiveness, their perceived risk of contracting H1N1, and whether they received a doctor's recommendation for the vaccine.
The dataset is structured to allow for detailed analysis, enabling the identification of patterns and relationships between these variables and vaccination behavior. Missing data is addressed using advanced imputation techniques, and categorical variables are transformed to facilitate analysis and modeling. By understanding this data, the project uncovers critical insights into the barriers and motivators of vaccine uptake, informing the development of effective public health strategies.

## EDA
The Exploratory Data Analysis (EDA) phase of the project focused on uncovering relationships and patterns within the dataset to gain insights into the factors influencing H1N1 vaccine uptake. Key findings include:
Impact of Doctor Recommendations:
- A strong correlation exists between receiving a doctor’s recommendation and vaccination.
- Individuals with a doctor’s recommendation were significantly more likely to get vaccinated compared to those without one.
     
Role of Health Insurance:
- Vaccination rates were higher among individuals with health insurance (27%) compared to those without (11%).
- This highlights healthcare access as a critical barrier to vaccine adoption.
    
Belief in Vaccine Effectiveness:
- A positive correlation was observed between belief in vaccine effectiveness and vaccination rates:
- Vaccination rates increased progressively with higher belief scores, peaking at 37% for the highest belief level.
    
Perceived Risk of H1N1 Infection:
- Vaccination rates rose with higher perceived risk of contracting H1N1:
- Individuals with the highest risk perception (score of 5) had vaccination rates of approximately 48%.
    
Key Insights from EDA:
- Doctor Recommendations and Health Coverage: These are critical drivers of vaccination and suggest targeted interventions.
- Perception Management: Public health campaigns can benefit from addressing vaccine skepticism and improving awareness of H1N1 risks and vaccine benefits.
  
The insights from EDA informed the subsequent modeling phase by highlighting the most influential variables and guiding feature engineering. These findings provide actionable directions for improving vaccination rates and shaping public health initiatives.

## Modelling
The modeling phase of the project focused on predicting H1N1 vaccine uptake using machine learning algorithms. Two models were developed and evaluated: a Decision Tree Classifier and Logistic Regression. Both models aimed to uncover patterns in the data and identify key factors influencing vaccination behavior.

Decision Tree Classifier:
- Achieved an Area Under the Curve (AUC) score of 0.84, indicating a good balance between true positives and false positives.
- Struggled with low precision and F1 scores, reflecting challenges in accurately predicting true vaccination behavior while minimizing false positives.
- The model demonstrated no signs of overfitting, making it suitable for generalization.
  
Logistic Regression:
- Also achieved an AUC score of 0.84, matching the Decision Tree’s ability to discriminate between vaccinated and non-vaccinated individuals.
- Precision and F1 scores remained low, consistent with the Decision Tree model.
- The simplicity and interpretability of Logistic Regression provide valuable insights into the relationship between predictors and vaccine uptake.
  
Key Takeaways:
- Both models performed better than the baseline, particularly in identifying influential factors driving vaccine uptake.
- While the AUC scores are strong, the models face challenges in precision and recall, indicating room for improvement.
- Future efforts will focus on refining these models, exploring additional features, and experimenting with advanced algorithms to improve predictive performance.
  
The insights gained from the modeling phase are valuable for understanding vaccination behavior and guiding public health strategies
## Conclusion, Reccommendation & Next steps 
The analysis offers several key recommendations for public health officials at the American Public Health Association (APHA):

- Promote Doctor Recommendations: Emphasizing the importance of doctor recommendations for the H1N1 vaccine could significantly boost vaccination rates.

- Ensure Vaccine Accessibility: Ensuring that the vaccine is accessible to all individuals, regardless of their health insurance status, is essential.

- Prioritize Educational Outreach: Focusing on educational initiatives that address perceptions of vaccine effectiveness and the perceived risk of H1N1 could positively influence vaccination uptake.

However, it's important to acknowledge the limitations in predicting H1N1 vaccination status, particularly in fully eliminating false negatives. Additionally, there may be unaccounted factors in the survey data that could impact vaccination prediction.

Looking ahead, analyzing more recent flu survey data and conducting further feature engineering could improve prediction accuracy. Moreover, extending predictions to include seasonal flu vaccine status could provide a more comprehensive understanding of vaccination behavior.
