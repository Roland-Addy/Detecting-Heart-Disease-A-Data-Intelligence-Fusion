# Detecting-Heart-Disease-A-Data-Intelligence-Fusion
This projects highlights the prevalence of heart diseases, particularly in the United States, where it's a leading cause of death, costing billions each year. The proposed data science solution introduces the application of machine learning to predict an individual's propensity for a heart attack. By analyzing health data and lifestyle factors, this approach offers early detection and personalized risk assessments. Furthermore, it has the potential to aid in the allocation of healthcare resources and even contribute to drug discovery.

## Problem Area
Heart and circulatory diseases is an umbrella term for all diseases of the heart and circulation. It includes everything from conditions that are inherited or that a person is born with, to those that develop later, such as coronary heart disease, atrial fibrillation, heart failure, stroke and vascular dementia. Globally it’s estimated that 1 in 13 people are living with a heart or circulatory disease.

In the United States, one person dies every 33 seconds from heart disease. It is the leading cause of deaths for people in most racial and ethnic groups in the country. In 2021, one in every 5 deaths was due to a heart disease. Unsurprisingly, this cost the US government about $239.9 billion each year from 2018 to 2019, including the cost of health care services, medicines, and lost productivity due to death. Heart disease is the leading cause of death for people of most racial and ethnic groups in the United States, including African American, American Indian, Alaska Native, Hispanic, and white men. For women from the Pacific Islands and Asian American, American Indian, Alaska Native, and Hispanic women, heart disease is second only to cancer.

Below are the percentages of all deaths caused by heart disease in 2021, listed by ethnicity, race, and sex:
| Race of Ethnic Group                     | % of Deaths   | 
|:-------------------                      |:--------------|
| American Indian or Alaska Native         | 15.5          | 
| Asian                                    | 18.6          | 
| Black (Non-Hispanic)                     | 22.6          | 
| Native Hawaiin or Other Pacific Islander | 18.3          | 
| White (Non-Hispanic)                     | 18.0          | 
| Hispanic                                 | 11.9          | 
| All	                                     | 17.4          | 


The most common heart disease is 'Coronary Artery Disease which killed 375,476 people in 2021. According to the Centers for Disease Control and Prevention (CDC), about 1 in 20 adults age 20 and older have Coronary Artery Disease, to put that into perspective, that is about 5% of adults age 20 and older. In 2021, about 2 in 10 deaths from Coronary Artery Disease, happen in adults less than 65 years old. Coronary heart disease can lead to a heart attack.

In the United States, someone has a heart attack every 40 seconds and every year about 805,000 people in the United States have a heart attack. Of these, 605,000 are a first heart attack. About 1 in 5 heart attacks are silent which means, the damage is done but the person is not aware of it. 

## Proposed Data Science Solution
High blood pressure, high blood cholesterol, and smoking are key risk factors for heart disease. Among these, several other medical conditions and lifestyle choices can also put people at a higher risk for heart disease. In healthcare, identifying and preventing the factors that have the greatest impact on heart disease is very important. Advances in technology have allowed the application of machine learning methods to detect "patterns" in the data, using these risk factors, that can predict a patient's condition or propensity to develop a heart disease.

This project seeks to apply machine learning techniques on a 2022 annual CDC survey data, of 400k+ adults related to their health status, to predict an individual's propensity to a heart attack. The ultimate goal of this project is to apply a number of machine learning methods, especially classifier models (logistic regression, SVM, random forest, etc.) to help make predictions of heart attacks.

## Impact of the solution
Significant impacts can be made in the healthcare industry by applying data science techniques in heart disease predictions. 
Firstly there will be early detection and risk assessment of heart disease. By applying a patient's data, medical history and lifestyle factors, a machine learning algorithm will be able to detect patterns that may not be immediately apparent to doctors or health care professionals allowing for fast medical interventions and allocation of health resources.
Secondly, this solution could allow for a personalized risk assessment. Machine learning models will be able to take into account a person's unique combination of risk factors, allowing for targeted interventions and prevention strategies, ensuring that high-risk individuals receive the most appropriate care.
Lastly, this solution could potentially be used in drug discovery.

## Data Description
The dataset originally comes from the Centers for Disease COontrol and Prevention (CDC) and is a major part of the Behavioral Risk Factor Surveillance System (BRFSS), which conducts annual telephone surveys to collect data on the health status of U.S. residents. As described by the CDC: "Established in 1984 with 15 states, BRFSS now collects data in all 50 states, the District of Columbia, and three U.S. territories. BRFSS completes more than 400,000 adult interviews each year, making it the largest continuously conducted health survey system in the world. The original dataset of nearly 300 variables was reduced by the author to 40 most relevant variables and that is what is used in this project.

Below is the Data Dictionary:

| Attributes/Variables                     | Survey Questions   | 
|:-------------------                      |:--------------|
| State                                    |The US State the respondent lives in         | 
| Sex                                      | Sex of Respondent         | 
| GeneralHealth                            | General Health of the respondent          | 
| PhysicalHealthDays                       | Now thinking about your physical health, which includes physical illness and injury, for how many days during the past 30 days was your physical health not good?          | 
| MentalHealthDays                         | Now thinking about your mental health, which includes stress, depression, and problems with emotions, for how many days during the past 30 days was your mental health not good?          | 
| LastCheckupTime                          | About how long has it been since you last visited a doctor for a routine checkup?          | 
| PhysicalActivities	                     | During the past month, other than your regular job, did you participate in any physical activities or exercises such as running, calisthenics, golf, gardening, or walking for exercise?          | 
| SleepHours	                             | On average, how many hours of sleep do you get in a 24-hour period?          |
| RemovedTeeth	                           | Not including teeth lost for injury or orthodontics, how many of your permanent teeth have been removed because of tooth decay or gum disease?          |
| HadHeartAttack (Target Variable)	       | (Ever told) you had a heart attack, also called a myocardial infarction?          |
| HadAngina                                |(Ever told) (you had) angina or coronary heart disease?        | 
| HadStroke                                |(Ever told) (you had) a stroke.        | 
| HadAsthma                                |(Ever told) (you had) asthma?          | 
| HadSkinCancer                            | (Ever told) (you had) skin cancer that is not melanoma?          | 
| HadCOPD                                  |(Ever told) (you had) C.O.P.D. (chronic obstructive pulmonary disease), emphysema or chronic bronchitis?          | 
| HadDepressiveDisorder                    | (Ever told) (you had) a depressive disorder (including depression, major depression, dysthymia, or minor depression)?          | 
| HadKidneyDisease	                       | Not including kidney stones, bladder infection or incontinence, were you ever told you had kidney disease?          | 
| HadArthritis	                           | (Ever told) (you had) some form of arthritis, rheumatoid arthritis, gout, lupus, or fibromyalgia?  (Arthritis diagnoses include: rheumatism, polymyalgia rheumatica; osteoarthritis (not osteporosis); tendonitis, bursitis, bunion, tennis elbow; carpal tunnel syndrome, tarsal tunnel syndrome; joint infection, etc.)|
| HadDiabetes	                             | (Ever told) (you had) diabetes?         |
| DeafOrHardOfHearing	                     | Are you deaf or do you have serious difficulty hearing?          |
| BlindOrVisionDifficulty                  | Are you blind or do you have serious difficulty seeing, even when wearing glasses?       | 
| DifficultyConcentrating                  | Because of a physical, mental, or emotional condition, do you have serious difficulty concentrating, remembering, or making decisions?        | 
| DifficultyWalking                        | Do you have serious difficulty walking or climbing stairs?       | 
| DifficultyDressingBathing                | Do you have difficulty dressing or bathing?          | 
| DifficultyErrands                        | Because of a physical, mental, or emotional condition, do you have difficulty doing errands alone such as visiting a doctor´s office or shopping?          | 
| SmokerStatus                             | Four-level smoker status:  Everyday smoker, Someday smoker, Former smoker, Non-smoker          | 
| ECigaretteUsage	                         | Would you say you have never used e-cigarettes or other electronic vaping products in your entire life or now use them every day, use them some days, or used them in the past but do not currently use them at all?| 
| ChestScan	                               | Have you ever had a CT or CAT scan of your chest area?          |
| RaceEthnicityCategory	                   | Five-level race/ethnicity category          |
| AgeCategory                              | Fourteen-level age category          |
| HeightInMeters                           | Reported height in meters       | 
| WeightInKilograms                        | Reported weight in kilograms       | 
| BMI                                      | Body Mass Index (BMI)         | 
| AlcoholDrinkers                          | Adults who reported having had at least one drink of alcohol in the past 30 days.        | 
| HIVTesting                               | Adults who have ever been tested for HIV         | 
| FluVaxLast12                             | During the past 12 months, have you had either flu vaccine that was sprayed in your nose or flu shot injected into your arm?         | 
| PneumoVaxEver	                           | Have you ever had a pneumonia shot also known as a pneumococcal vaccine?          | 
| TetanusLast10Tdap	                       | Have you received a tetanus shot in the past 10 years? Was this Tdap, the tetanus shot that also has pertussis or whooping cough vaccine? |
| HighRiskLastYear                         | You have injected any drug other than those prescribed for you in the past year. You have been treated for a sexually transmitted disease or STD in the past year. You have given or received money or drugs in exchange for sex in the past year. |
| CovidPos                                 | Has a doctor, nurse, or other health professional ever told you that you tested positive for COVID 19?        |


The dataset can be found [here on Kaggle](https://www.kaggle.com/datasets/kamilpytlak/personal-key-indicators-of-heart-disease/data)


## Project Organization
* Step 1: Exploratory Data Analysis
* Step 2: Data Preprocessing
* Step 3: Fitting Baseline Models

### Exploratory Data Analysis
* The dataset contains 445,132 instances with 40 variables.
* There were 157 duplicated instances and missing values in 38 out of the 40 columns.
* There is a significant class imbalance in the dataset. 

Notably the below are significant in determining an individual’s odds in having a heart attack:
* The sex
* Number of days where an individual's physical health was not good
* The number of days where an individual's mental health was not good
* The average number of sleep hours in a day
* An individual's height and weight

### Data Preprocessing
* The duplicated instances were removed.
* Missing Values in the dataset were resolved.
* Multicolinearity was detected in the data, which was rectified using the Variance Inflation Factors.
* After data preprocessing, there are 111 features to work with.

### Fitting Baseline Models
* The dataset was split into train and test sets. The train set was upsampled to resolved the class imbalance.
* Due to the class imbalance in the test set and the nature of the target variable, the AUC Score metric was used in the model evaluation.
* The below base models were used using grid searching over a range of hyperparameters:
* * Logistic Regression - AUC Score of 0.88
  * Decision Tree Classifier - 

