# Nutrition, Physical Activity, and Obesity Analysis - Behavioral Risk Factor Surveillance System

## Dataset Description
This project analyzes the **Nutrition, Physical Activity, and Obesity - Behavioral Risk Factor Surveillance System (BRFSS)** dataset. This dataset provides information on behavioral risk factors that impact public health, such as physical activity levels, nutrition, and obesity trends across different demographics in the United States.

The dataset can be accessed from the following URL: [Dataset](https://raw.githubusercontent.com/Jerald011003/Nutrition-Physical_Activity-and-Obesity-Analysis/refs/heads/main/Nutrition__Physical_Activity__and_Obesity_-_Behavioral_Risk_Factor_Surveillance_System.csv).

### Data Columns and Descriptions
- **YearStart**: Starting year of data collection for a particular record.
- **YearEnd**: Ending year of data collection for the record (usually the same as `YearStart`).
- **LocationAbbr**: Abbreviation of the location (e.g., state or region).
- **LocationDesc**: Full description of the location.
- **Datasource**: The data source or system from which the data is collected.
- **Class**: High-level category of the topic (e.g., "Nutrition", "Physical Activity").
- **Topic**: Specific topic within the class (e.g., "Fruit Consumption", "Exercise Frequency").
- **Question**: Survey question asked to gather the data.
- **Data_Value_Unit**: Unit of measurement for the data value (e.g., percentage).
- **Data_Value_Type**: Type of data value (e.g., "Mean", "Percentage").
- **Data_Value**: Collected data value based on the question.
- **Data_Value_Alt**: Alternate form of the data value, if applicable.
- **Data_Value_Footnote_Symbol**: Symbol indicating a footnote related to the data value.
- **Data_Value_Footnote**: Footnote text providing additional context or clarification about the data value.
- **Low_Confidence_Limit**: Lower bound of the confidence interval for the data value.
- **High_Confidence_Limit**: Upper bound of the confidence interval for the data value.
- **Sample_Size**: Number of survey respondents used to calculate the data value.
- **Total**: Aggregate total for the specific category or group.
- **Age(years)**: Age group of respondents, measured in years.
- **Education**: Education level of respondents.
- **Gender**: Gender of respondents.
- **Income**: Income level of respondents.
- **Race/Ethnicity**: Race or ethnicity of respondents.
- **GeoLocation**: Geographic coordinates (latitude and longitude) of the location.
- **ClassID**: Unique identifier for the class category.
- **TopicID**: Unique identifier for the topic.
- **QuestionID**: Unique identifier for the question.
- **DataValueTypeID**: Unique identifier for the data value type.
- **LocationID**: Unique identifier for the location.
- **StratificationCategory1**: Category used for stratification (e.g., age, gender).
- **Stratification1**: Specific stratification within the category (e.g., "Male" or "Female").
- **StratificationCategoryId1**: Unique identifier for the stratification category.
- **StratificationID1**: Unique identifier for the specific stratification.

## Summary of Findings
1. **Physical Activity and Obesity**: Trends indicate that lower physical activity is associated with higher obesity rates.
2. **Diet and Obesity**: Individuals with poor dietary habits showed a higher prevalence of obesity.
3. **Demographics and Health Risk**: Obesity rates vary significantly by age, gender, and region.

## Data Preprocessing
Preprocessing steps included:
- Handling missing values using `SimpleImputer`.
- Label encoding categorical variables with `LabelEncoder`.
- Standardizing numerical data using `StandardScaler` for consistency across features.

## Exploratory Data Analysis
Initial analysis involved statistical summaries and visual inspections to understand the relationships between physical activity, diet, and obesity levels. Key observations highlighted demographic patterns in health behaviors and outcomes.

## Visualization
Various visualizations were created to illustrate findings:
- **Distribution Plots**: Illustrated demographic differences in obesity and physical activity.
- **Correlation Heatmaps**: Showed relationships between various health factors.
- **Bar Charts and Histograms**: Displayed data distributions across different demographic groups.

Each visualization includes interpretations that provide context and insights derived from the data.

## Model Development
The following models were developed to predict obesity and assess factors affecting physical health:
1. **Logistic Regression**
2. **Support Vector Classifier (SVC)**
3. **Random Forest Classifier**
4. **Gradient Boosting Classifier**

Each model was fine-tuned using `GridSearchCV` to optimize performance based on accuracy and other relevant metrics.

## Model Evaluation
Each model was evaluated individually using the following metrics:
- **Accuracy Score**: A primary measure of model correctness.
- **Classification Report**: Detailed breakdown of precision, recall, and F1 score.
- **Confusion Matrix**: Visualization of true vs. predicted values for each class.

## Conclusion
This project provides a comprehensive analysis of the BRFSS dataset, identifying key behavioral risk factors associated with obesity. The developed models offer insights into public health risks, which can guide preventive measures and policy decisions.

## Contributors
- **Jerald Francis Bagsic**: Data analysis, model development, and documentation.
