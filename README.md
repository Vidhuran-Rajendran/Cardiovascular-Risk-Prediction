# project3-Cardiovascular-Risk-Prediction

## 📋 <b> Problem Description </b>

The dataset is from an ongoing cardiovascular study on residents of the town of Framingham,
Massachusetts.

The classification goal is to predict whether the patient has a 10-year risk of
future coronary heart disease (CHD). 

The dataset provides the patients’ information. It includes
over 4,000 records and 15 attributes.
Variables
Each attribute is a potential risk factor. There are both demographic, behavioral, and medical risk
factors.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 📋 <b> Data Description </b>

### **Demographic:**
* Sex: male or female("M" or "F")
* Age: Age of the patient;(Continuous - Although the recorded ages have been truncated to whole numbers, the concept of age is continuous)

### **Behavioral**
* is_smoking: whether or not the patient is a current smoker ("YES" or "NO")
* Cigs Per Day: the number of cigarettes that the person smoked on average in one day.(can be
considered continuous as one can have any number of cigarettes, even half a cigarette.)

### **Medical( history)**
**BP Meds**: whether or not the patient was on blood pressure medication (Nominal)

**Prevalent Stroke**: whether or not the patient had previously had a stroke (Nominal)

**Prevalent Hyp**: whether or not the patient was hypertensive (Nominal)

**Diabetes**: whether or not the patient had diabetes (Nominal)
Medical(current)

**Tot Chol**: total cholesterol level (Continuous)

**Sys BP**: systolic blood pressure (Continuous)

**Dia BP**: diastolic blood pressure (Continuous)

**BMI**: Body Mass Index (Continuous)

**Heart Rate**: heart rate (Continuous - In medical research, variables such as heart rate though in
fact discrete, yet are considered continuous because of large number of possible values.)

**Glucose**: glucose level (Continuous)
Predict variable (desired target) 

**10-year risk of coronary heart disease CHD(binary: “1”, means “Yes”, “0” means “No”) -DV**

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 📖 Approach:-
### Data preparation:
•	Removed null values from the dataset

•	Removed duplicate entries

•	Used SMOTE and random under sampling to get a balanced dataset

### Feature engineering:
•	Extracted feature ‘Hypertension’ from systolic and diastolic blood pressure data

•	Extracted feature ‘Diabetese severity’ from diabetes and glucose column

•	Constructed new feature ‘Smoking Factor’ from number of cigarettes consumption

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 📖 XGBoost
XGBoost (extreme Gradient Boosting) is an advanced implementation of the gradient boosting algorithm. XGBoost has proved to be a highly effective ML algorithm, extensively used in machine learning competitions and hackathons. XGBoost has high predictive power and is almost 10 times faster than the other gradient boosting techniques. It also includes a variety of regularization which reduces overfitting and improves overall performance.

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 📋 Conclusion:-

Using XGBoost and finetuning parameters with grid search and cross-validation I got a Recall of 94%

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

<h2 id="credits"> :scroll: Credits</h2>

< Vidhuran Rajendran > | Avid Learner | Data Scientist | Machine Learning Engineer | Deep Learning enthusiast

<p> <i> Contact me for Data Science Project Collaborations</i></p>

[![LinkedIn Badge](https://img.shields.io/badge/LinkedIn-0077B5?style=for-the-badge&logo=linkedin&logoColor=white)](www.linkedin.com/in/vidhuran)
[![GitHub Badge](https://img.shields.io/badge/GitHub-100000?style=for-the-badge&logo=github&logoColor=white)](github.com/Vidhuran-Rajendran)
[![Medium Badge](https://img.shields.io/badge/Medium-1DA1F2?style=for-the-badge&logo=medium&logoColor=white)](https://medium.com/@vidhuran_07)
[![Resume Badge](https://img.shields.io/badge/resume-0077B5?style=for-the-badge&logo=resume&logoColor=white)](https://drive.google.com/file/d/1pp1bqy3GPgYD-XH0CjP9B7SoUzQnwSsN/view?usp=sharing)

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)

## 📚 References
1. Coronary Heart Disease - https://www.medicalnewstoday.com/articles/184130
2. Pulse Pressure - https://www.mayoclinic.org/diseases-conditions/high-blood-pressure/expert-answers/pulse-pressure/faq-20058189#:~:text=The%20top%20number%20(systolic)%20minus,40%20mm%20Hg%20is%20unhealthy.
3. Using SMOTE - https://machinelearningmastery.com/smote-oversampling-for-imbalanced-classification/
4. XGBoost Documentation - https://xgboost.readthedocs.io/en/stable/

![-----------------------------------------------------](https://raw.githubusercontent.com/andreasbm/readme/master/assets/lines/rainbow.png)
