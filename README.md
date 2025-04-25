📁 Dataset Overview
Source: Titanic survival dataset (Kaggle)

Features:

Categorical: Sex, Embarked, Pclass

Numerical: Age, Fare, SibSp, Parch

Target: Survived (0 = No, 1 = Yes)

🧹 Preprocessing Steps
1. 🔍 Import & Explore the Dataset
Loaded the dataset using pandas

Inspected data types, null values, and basic structure with info() and describe()

2. 🧩 Handle Missing Values
Age: Replaced missing values using mean imputation

Embarked: Used mode imputation

Dropped Cabin due to high missingness

3. 🔤 Categorical Encoding
Converted Sex and Embarked into numerical values using Label Encoding

4. ⚖️ Feature Normalization
Applied StandardScaler to normalize numerical features like Age and Fare

📊 Exploratory Data Analysis (EDA)
1. Generate Summary Statistics
Calculated basic summary statistics for numerical features, including mean, median, and standard deviation.

2. Distribution Plots
Created histograms to visualize the distribution of key numerical features: Age, Fare, SibSp, and Parch.

Generated boxplots to detect outliers and visualize the spread of numerical features.

3. Correlation Matrix & Heatmap
Generated a correlation matrix to understand relationships between numerical features.

Visualized the correlation matrix using a heatmap to detect any strong correlations.

4. Pairplot of Key Features
Created a pairplot to explore the pairwise relationships between features such as Age, Fare, Pclass, and survival (Survived).

5. Group-Based Visualizations
Used count plots to explore survival rates based on categorical features like Sex, Pclass, and Embarked.

Created bar plots for visualizing survival rates within different fare ranges and passenger classes.

🧑‍💻 Technical Stack
Libraries Used:

pandas: For data manipulation

numpy: For numerical computations

matplotlib: For plotting visualizations

seaborn: For statistical visualizations (boxplots, pairplots, etc.)

📈 Insights
Age & Survival Rate: Younger passengers tend to have a higher survival rate, especially those under 10 years old.

Fare & Survival Rate: Passengers who paid higher fares had a better chance of survival.

Pclass & Survival Rate: First-class passengers had the highest survival rate, while third-class passengers had the lowest.

Sex & Survival: A significantly higher proportion of females survived compared to males.

