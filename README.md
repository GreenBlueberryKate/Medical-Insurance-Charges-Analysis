# Project Conclusion — Medical Insurance Charges Analysis

🎯 Objective

The goal of this project was to understand which demographic and lifestyle factors most strongly influence individual medical insurance charges. Rather than focusing on complex modeling techniques, the analysis emphasized exploratory data analysis (EDA), statistical reasoning, and interpretable linear regression.

🔎 Key Exploratory Insights

Initial analysis revealed that insurance charges are heavily right-skewed, indicating that a small subset of individuals accounts for disproportionately high medical expenses.

Behavioral segmentation uncovered a strong structural pattern:

Smoking status emerged as the most influential driver of insurance costs.

Charges increased steadily across age bands, but smoking shifted the entire cost distribution upward.

BMI showed a gradual positive relationship with charges, suggesting a compounding lifestyle effect rather than a sudden cost jump.

When combining age and smoking, smokers consistently exhibited dramatically higher costs across all life stages, highlighting the interaction between demographic and behavioral risk factors.

📊 Modeling Approach

A linear regression model was developed to quantify how these variables contribute to insurance pricing.

Key modeling decisions:

Categorical variables were encoded using one-hot encoding.

The model focused on interpretability rather than predictive complexity.

Performance was evaluated using R² and Mean Absolute Error (MAE).

📈 Model Performance

R² (Test): ~0.80
The model explains approximately 80% of the variation in insurance charges, indicating strong explanatory power for a baseline linear model.

MAE: ~4,266
On average, predictions differ from actual charges by about $4k, which is reasonable given the wide range of expenses.

These results suggest that a small set of demographic and lifestyle variables captures much of the pricing structure.

💡 Key Analytical Findings

Smoking status introduces a substantial cost increase (~$23k on average), making it the dominant predictor.

Age contributes a steady incremental rise in expected charges.

BMI has a consistent positive effect, reflecting gradual health risk accumulation.

Regional and gender effects appear comparatively modest.

Overall, the analysis highlights how behavioral factors can outweigh purely demographic attributes in determining healthcare expenses.

🛠️ Tools Used

Python · Pandas · Matplotlib · Scikit-learn
