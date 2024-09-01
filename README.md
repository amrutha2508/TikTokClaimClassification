## TikTok Claim Classification 

**Objective:** Developed a machine learning model to classify TikTok videos as either claims or opinions to optimize the moderation process and reduce the backlog of user reports.

**Data Overview:** Worked with a dataset containing five float64, three int64, and four object-type features with 19,382 observations. Addressed missing values, outliers, and multicollinearity issues.

**Exploratory Data Analysis (EDA):** Identified significant relationships between claim status and engagement metrics. Analyzed distribution patterns and engagement rates among different author ban statuses and video types.

**Feature Engineering:** Applied log transformations and selective outlier imputations to key engagement metrics like video views, likes, comments, shares, and downloads to improve model stability and reduce multicollinearity.

**Model Development:** Built and evaluated multiple models, including Logistic Regression, Random Forest, and XGBoost, using cross-validation to optimize hyperparameters.

**Performance:** Achieved high recall (0.995) with the Random Forest model, identifying claims and opinions with near-perfect precision and F1-scores. Ensured the model minimized false negatives to prioritize reviewing potential claim violations effectively.

**Feature Importance:** Determined that features related to video engagement levels (e.g., views, likes, shares) were the most predictive of claim status, aligning with findings from EDA.

**Business Impact:** Enabled automated prioritization of videos for moderation, potentially improving the efficiency of human reviewers and ensuring that videos violating terms of service are more effectively identified.

**Technologies Used:** Python, scikit-learn, XGBoost, Random Forest, Logistic Regression, CountVectorizer for text feature engineering, and statistical analysis tools.

**Outcome:** Delivered a robust classification model with excellent recall and precision, suitable for real-world application to enhance TikTok's moderation process.

Follow the jupyter notebooks in the following order: tiktokEDA, TikTokLogisticRegression, TikTokRFXBG

TikTokMLR is some extra analysis: preditive model for predicting whether a user is verified or not.
