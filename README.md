### Project Title
Student Depression Analysis
**Author**
MEI ZHONG
#### Executive summary
Understanding and addressing student depression is critical in today’s academic and social landscape. This project investigates the factors that contribute to depression among students and develops a predictive model for early intervention. By identifying patterns in student behavior, lifestyle, and background, the project aims to support proactive mental health strategies within educational institutions.
#### Rationale
Depression among students is a growing concern affecting both academic performance and personal well-being. Without early detection and intervention, students may face long-term psychological, emotional, and academic challenges. This analysis provides data-driven insights that can help educators, counselors, and policymakers design better mental health support systems, reduce dropout rates, and improve student outcomes.

#### Research Question
What are the key factors contributing to depression among students, and how can they be used to predict depression levels for early intervention?

#### Data Sources
The analysis uses the Student Depression Dataset from Kaggle, which includes multidimensional data such as:

Demographics

Academic performance

Lifestyle habits (sleep, exercise, screen time)

Family mental health history

Self-reported depression status

#### Methodology
To prepare the data for modeling, a variety of encoding and transformation techniques were applied depending on the nature of each feature:

- binary encoding 
- label encoding 
- one-hot encoding
- binary flag
- use as-is
- standardization
- ordinal encoding
- group and ordinal encoding

A set of baseline classification models was implemented to predict student depression status:

- Neural Network
- Logistic Regression
- SVC
- Decision Tree

To assess model performance, a comprehensive set of classification metrics was used:

- Accuracy
- Precision
- Recall
- F1-score
- ROC/AUC

#### Results
- All models perform very well
    - AUC values above 0.85 indicate strong classification power.
    - All models separate the classes (Depressed vs Not) significantly better than random guessing (AUC = 0.5).
- Best Performers: Logistic Regression & SVC
    - Both reach AUC = 0.89, meaning they strike the best balance between true positives and false positives across all thresholds.
    - These two may be preferred if interpretability (logistic) or margin-based confidence (SVC) matters.
- Neural Network vs Decision Tree
    - Slightly lower AUC (0.88) but still competitive.
    - Neural Networks may capture non-linearities, while Decision Trees are easier to interpret.
    - Slightly steeper initial lift in the curve suggests they catch more positives early, but plateau faster.

#### Next steps
Model Improvement: Fine-tune models using hyperparameter tuning and advanced algorithms (e.g., Random Forest, XGBoost).
Intervention Design: Work with educators and counselors to convert model outputs into real-world support tools.
Longitudinal Tracking: Explore longitudinal datasets to track student mental health over time.


##### Contact and Further Information

Mei Zhong
miazhong0801@gmail.com
https://github.com/meizhong0801/UC-Berkeley-capstone-project/tree/main