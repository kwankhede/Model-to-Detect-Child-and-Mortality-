# Fetal Health Classification Project

## Abstract
Develop a model to classify fetal health to prevent child and maternal mortality using features extracted from Cardiotocogram exams.

Reducing child mortality is a key indicator of human progress, aligning with the United Nations' Sustainable Development Goals. By 2030, the goal is to end preventable deaths of newborns and children under 5 years, with a target of reducing under-5 mortality to at least 25 per 1,000 live births. Maternal mortality, another critical aspect, accounts for a significant number of deaths, mostly preventable, occurring during and after pregnancy.

Cardiotocograms (CTGs) provide a simple and cost-effective means to assess fetal health. They offer valuable insights into fetal heart rate (FHR), fetal movements, uterine contractions, and more, enabling healthcare professionals to take preventive actions.

## Data
The dataset comprises 2126 records with features extracted from Cardiotocogram exams, classified by three expert obstetricians into three classes: Normal, Suspect, and Pathological. The distribution shows approximately 77.8% of instances labeled as "Normal," 13.90% as "Suspect," and 8.28% as "Pathological," indicating a predominantly healthy dataset with a small proportion requiring further scrutiny.

## Feature Description
- baseline value: Fetal heart rate baseline (beats per minute)
- accelerations: Number of accelerations per second
- fetal_movement: Number of fetal movements per second
- uterine_contractions: Number of uterine contractions per second
- light_decelerations: Number of light decelerations per second
- severe_decelerations: Number of severe decelerations per second
- prolonged_decelerations: Number of prolonged decelerations per second
- abnormal_short_term_variability: Percentage of time with abnormal short-term variability
- mean_value_of_short_term_variability: Mean value of short-term variability
- percentage_of_time_with_abnormal_long_term_variability: Percentage of time with abnormal long-term variability
- mean_value_of_long_term_variability: Mean value of long-term variability
- histogram_width: Width of FHR histogram
- histogram_min: Minimum of FHR histogram
- histogram_max: Maximum of FHR histogram
- histogram_number_of_peaks: Number of FHR histogram peaks
- histogram_number_of_zeroes: Number of FHR histogram zeroes
- histogram_mode: FHR histogram mode
- histogram_mean: FHR histogram mean
- histogram_median: FHR histogram median
- histogram_variance: FHR histogram variance
- histogram_tendency: FHR histogram tendency

## Target Variable
- fetal_health: Fetal state class code (1=Normal, 2=Suspected, 3=Pathological)

## Considered Modeling Algorithms
- Naive Bayes
- Logistic Regression
- Decision Tree
- Random Forest with hyperparameter tuning
- Support Vector Machines (SVM)
- Gradient Boosting Classifier with hyperparameter tuning

These algorithms are explored to identify the most suitable model for the given task.

## Observation
After hyperparameter tuning, both **Random Forest** and **Gradient Boosting** models demonstrated improvements across various performance metrics. The tuned *Random Forest* model exhibited enhanced precision, recall, and F1 Score, resulting in an overall accuracy boost. Similarly, the *Gradient Boosting* model, after tuning, showcased improved precision, recall, and F1 Score, indicating increased effectiveness in classifying instances. The results affirm the positive impact of hyperparameter optimization on model performance.
