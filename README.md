# End to End Machine Learning Project

when we are building a machine learning solution first we should asnwer following questions:
* what questions are we trying to answer? Do we think the data collected can answer that question
* What is the best way to phrase our questions as a machine learning problem?
* Have we collected enough data to represent the problem want to solve?
* what features of the data did we extract, and will these enable the right predictions?
* How will we measure success in our application?


## Real World Problem
In today’s world, chronic lifestyle-related diseases (such as heart disease, diabetes, obesity, and certain cancers) are rising rapidly due to poor lifestyle habits — unhealthy diets, lack of exercise, inadequate sleep, stress, smoking, and alcohol consumption.

The challenge is that:
* Many peaople don't know they are at a high risk until it's too late.
* Healhcare systems aspend billions on trating preventable conditions.
* Preventive health screenings are not personalized enough for individual's lifestyles.
**Our project** aims to use **Machine Learning** to predict disease risk **early**, enabling people and healthcre providers to take actions before a disease develops.


Who benefits from Solving This problem?
1. individuals/Patients
      * gain awareness of their personal health risks.
      * can make targeted lifestyle changes to prevent illness.
      * Reduce long term medical costs and improve quality of life.
2. Healthcare Providers & Doctors
      * can identify at-risk patients earlier.
      * Focus on prevention rather than only tratment.
      Offer more personalized healthcare plans.
3. Public Health Organizations & Governments
      * Can design more effective disease prevention campaigns.
      * Reduce healthcare system burden and costs.
      * Allocate resources more efficiently.
4. insurance Companies
      * Predict risk profiles for better policy planning.
      * Offer incentives for health lifestyle changes.
5. Employers
      * Support employee wellness programs.
      * Reduce sick leaves and improve productivity.





Answers for main questions arise when building machine learning solution:

1. **What questions are we trying to answe?**
      * Can we predict the *likelihood of a person developing a disease* based on their daily habits, health metrics, demographics, and psychological indicators?
      * Which lifestyle factors contribute most to disease risk?
      * Can this prediction be made early enough to allow preventive interventions?
2. **Do we think the data collected can answer that question?**
    Yes — the dataset contains lifestyle, biometric, demographic, and mental health features known to influence chronic disease risk. These are supported by real-world research (e.g., Framingham Heart Study, WHO lifestyle risk factors).
However, we must check:
      * *Data completeness*(missing values)
      * *Class balance*(enough positive and negative cases)
      * *Quality*(no unrealistic or noisy values)
3. **What is the best way to phrase our question as a machine learning problem?**
      * *Type*: Supervised classification problem
      * *Input*: Numerical and categorical features(habits,biometrics,demographics,mental heal indicator)
      * *Output*: Binary classification -> `1`=high disease risk, `0`=low disease
      * *Goal*: maximize model accuarcy while maintaining good recall for high-risk cases
4. **Have we collected enough data to represent the problem we want to solve?**
      * The dataset size must be large enough to capture variability in human lifestyle patterns across different ages, genders, and health conditions.
      * We should verify the dataset has *balanced representation* of both healthy and high-risk individuals to avoid bias.
      * If the dataset is small or imbalanced, we may need data augmentation or additional data sources.
5. **What features of the data did we extract, and will these enable the right predictions?**
    Key Features:
      * *Lifestyle*: diet, physical activity, smoking, alcohol use, sleep
      * *Biometrics*: BMI, blood pressure, cholesterol, glucose
      * *Demographics*: age, gender
      * *Psychological factors*: stress, mental health indicators.

These eatures align with known risk factors from medical studies, making them strong predictors for our problem.


6. **How will we measure success in our application?**
    * Primary Metrics:
      * *Accuracy* — overall correct predictions
      * *Precision & Recall* — especially recall for high-risk cases (to minimize false negatives)
      * *AUC-ROC* — ability to separate high-risk from low-risk individuals

    * Secondary measures:
      * Interpretability of the model for healthcare professionals
      * Usability in a real-world preventive healthcare setting

Information about the dataset
link: https://www.kaggle.com/datasets/mahdimashayekhi/disease-risk-from-daily-habits
size = 100000 rows


Group members and roles
IT24104083 - Wijesinghe P.H.G.T.P -  Handling Missing data
IT24103606 - Rathnayake R.M.P.T - Categorical feature encoding
IT24101992 - Vaishmitha M - Numerical Feature scaling
IT24103081 - Rathnayake M.D.Y.B - Dimensionality reduction and feature selection
IT24610808 - Ekanayake E.W.M.W.W.T.D.B - Feature Engineering
IT24102905 - Gunawardana B.P.P.G.D.S - Outlier Removal

