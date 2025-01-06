# The Future of Education: Predicting Student Performance with Data Science

## Business Case

In the education sector, understanding student performance trends is essential for evaluating the effectiveness of educational programs and policies. By accurately predicting and categorizing student performance levels, educational institutions can make data-driven decisions to improve retention, graduation rates, and overall student success. This project aims to develop a machine learning model that predicts the "reg_pct_level" (student performance level) based on various features such as enrollment counts, graduation rates, and dropout rates.

## Key Steps Taken to Solve the Problem

### 1. **Dataset Understanding**
   - The first step involved thoroughly understanding the dataset, which included analyzing the features and the target variable: `reg_pct_level`.
   - The dataset contained features like enrollment count (`enroll_cnt`), graduation count (`grad_cnt`), graduation percentage (`grad_pct`), and dropout count (`dropout_cnt`).

### 2. **Data Preprocessing**
   - **Handling Missing Values**: Missing data was addressed through appropriate imputation techniques.
   - **Encoding Categorical Variables**: Categorical variables were encoded into numerical values for model compatibility.
   - **Feature Scaling**: Data scaling techniques were applied where necessary to standardize numerical features.

### 3. **Model Selection and Training**
   - Initially, two types of models were evaluated: **Decision Trees** and **Random Forests**.
   - Four models were trained and evaluated:
     - **Decision Tree Model 1**
     - **Decision Tree Model 2**
     - **Random Forest Model 1**
     - **Random Forest Model 2**
   - Cross-validation was performed on the training dataset to evaluate the models’ performance using accuracy as the primary metric.

### 4. **Cross-Validation and Model Evaluation**
   - The models were evaluated using 5-fold cross-validation, and the mean accuracy score for each model was computed.
   - **Random Forest Model 1** outperformed all other models with the highest average accuracy of **91.49%** during cross-validation.

### 5. **Model Testing**
   - The best-performing model (**Random Forest Model 1**) was applied to the testing dataset.
   - The model's performance on the test data was evaluated using a classification report, indicating a strong balance of **precision**, **recall**, and **F1-score** across different performance categories.

### 6. **Model Selection**
   - Based on the cross-validation results and testing performance, **Random Forest Model 1** was selected as the preferred model for predicting student performance trends.
   - The final model achieved an accuracy of **92%** on the testing subset.

### 7. **Performance Analysis**
   - The final model performed well across all classes, making it reliable for predicting performance trends.
   - The accuracy and balanced metrics confirmed the robustness of the model in generalizing to unseen data.

### 8. **Discussion on Model Selection**
   - **Random Forest** was preferred for its better performance, compared to the Decision Trees, and its balance between accuracy and interpretability.
   - Though **accuracy** was the main evaluation metric, factors like **model interpretability** were also taken into account.

## Business Recommendations

- **Targeted Interventions**: The model can be used to identify at-risk students early on, allowing for targeted interventions to improve retention and graduation rates.
- **Resource Allocation**: Insights gained from the predictions can guide institutions in allocating resources effectively, focusing efforts on students who are more likely to need support.
- **Policy Improvements**: Educational policies can be refined by understanding performance trends, allowing institutions to implement data-driven changes to improve student outcomes.

## Conclusion

The project successfully demonstrates the power of machine learning to analyze and predict student performance trends based on historical data. By selecting the most accurate and reliable model, the project highlights the potential of data-driven decision-making in the educational domain. Further enhancements could include exploring additional features, fine-tuning model parameters, and incorporating other machine learning techniques to improve model accuracy.

## Future Work

- **Hyperparameter Tuning**: Fine-tuning hyperparameters of the Random Forest model to optimize performance.
- **Feature Engineering**: Exploring more advanced feature engineering techniques to capture deeper insights from the data.
- **Other Algorithms**: Experimenting with alternative algorithms like Gradient Boosting or XGBoost to compare performance and further improve predictions.

## Author

**Ansuman Patnaik**  
MS in Data Science & Analytics, Yeshiva University  
Email: ansu1p89k@gmail.com
