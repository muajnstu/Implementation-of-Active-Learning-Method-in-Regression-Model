# Implementation-of-Active-Learning-Method-in-Regression-Model
 Active learning is a specialized branch of machine learning that aims to improve model
 efficiency by reducing the amount of labeled data required for training. It identifies
 and prioritizes the most informative or uncertain samples for labeling, ensuring that
 each labeled data point maximally contributes to the model’s performance. Active
 learning operates iteratively, where the model learns from labeled data, identifies
 areas of high uncertainty, and requests labels for those specific data points.
 In predicting medical insurance costs, active learning can prioritize cases where the
 relationship between variables (e.g., BMI and medical charges) is ambiguous. For
 example, a non-smoker with a high BMI might yield a wide range of potential costs,
 making their data point particularly informative for labeling.

We used three open-source datasets to predict health insurance premiums.

Dataset 1 was sourced from Kaggle and contains 1,334 entries with seven features, mainly related to demographics and lifestyle. It includes three categorical features: Sex, Gender, and Location. The first two were encoded using label encoding, while Location was processed using one-hot encoding. The other columns are made up of integer and continuous values. There were no missing values, so none were removed, but a duplicate entry was found and deleted. This dataset has been used in several studies, including those by Ulhasan and Sijie.

Dataset 2, also from Kaggle, is known as the Indian Health Insurance Dataset. It's referenced in academic literature and offers slightly better predictive features than Dataset 1. It has 11 features and around 1,000 entries, all integers. There are no missing or duplicate values in this dataset.

Dataset 3 contains health and habit-related data. It includes 24 features across 25,000 records. The data is mostly integers, with eight categorical and two continuous variables. An unnecessary column called application_id was removed. Two columns had missing values, which were filled in using their mean. The column cholesterol_level originally contained ranges like “700–800”, which were replaced by the average value of each range. Most categorical features were encoded through simple mapping. However, since Location had many unique values, it was processed using target encoding. The dataset was generously shared by data scientist G. Deepak Reddy.

 

