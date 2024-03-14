# StudentMentalHealth

A STATISTICAL RESEARCH ON THE EFFECTS OF MENTAL HEALTH ON STUDENTS’ CGPA

Data Preprocessing:

The 'Timestamp' column was dropped as it was not relevant for the analysis.
Missing values in the 'Age' column were filled with the median age, and the column was converted to integer type.
Categorical variables were one-hot encoded to enable modeling.

Model Building:

A Random Forest classifier was trained on the preprocessed data to predict whether individuals sought specialist treatment.
Hyperparameter tuning was performed using grid search with 5-fold cross-validation to optimize the model's performance.

Model Evaluation:

The tuned Random Forest classifier achieved an accuracy of 90% on the test set.
The classification report revealed high precision, recall, and F1-score for the 'No' class (Did not seek specialist treatment), indicating good performance in predicting instances where specialist treatment was not sought.
However, the model performed poorly for the 'Yes' class (Sought specialist treatment), with precision, recall, and F1-score all being 0.00. This suggests that the model failed to predict instances where specialist treatment was sought correctly.

Recommendations for Improvement:

Addressing the class imbalance by collecting more data or using advanced techniques like SMOTE to balance the classes could improve the model's performance.
Exploring additional features related to healthcare and patient records could provide more information for predicting specialist treatment-seeking behavior.
Experimenting with different machine learning algorithms and ensemble methods may lead to better predictive performance.
Collaborating with healthcare professionals to incorporate domain knowledge and insights could help refine the model and make it more clinically relevant.
In conclusion, while the initial model shows promise in predicting instances where specialist treatment was not sought, 
further refinement and enhancements are needed to improve its ability to predict instances where specialist treatment was sought, 
ultimately making it more useful for proactive healthcare interventions.
