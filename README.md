# Diamond-Dynamics
Diamond Dynamics is a machine learning project that predicts diamond prices and segments diamonds into market categories using physical and quality attributes like carat, cut, color, and clarity. It includes EDA, feature engineering, regression models, ANN, clustering, and a Streamlit app for real-time price and cluster prediction

Project Workflow – Step by Step
1️⃣ Data Collection

Used the Diamond Dataset containing 53,940 rows and 10 features

Features include carat, cut, color, clarity, dimensions (x, y, z), and price

Target variable: Diamond Price (converted from USD to INR)

2️⃣ Data Cleaning & Preprocessing

Checked for missing values and data inconsistencies

Converted zero or invalid values in x, y, and z columns to null and handled them

Removed irrelevant or redundant columns if necessary

Converted price from USD to INR using a fixed conversion rate

3️⃣ Exploratory Data Analysis (EDA)

Analyzed distributions of numerical features (price, carat, x, y, z)

Visualized categorical features (cut, color, clarity) using count plots

Studied price variation across carat, cut, color, and clarity using boxplots

Generated correlation heatmaps to identify relationships among numerical features

Used scatter plots and pair plots to understand feature interactions

4️⃣ Outlier Detection & Skewness Handling

Identified outliers using IQR and Z-Score methods

Verified outliers visually using boxplots

Reduced skewness in highly skewed features (price, carat, dimensions) using

Log transformation

Square root / Box-Cox transformation

5️⃣ Feature Engineering

Created new meaningful features:

Volume = x * y * z

Price per Carat

Dimension Ratio

Carat Category (Light, Medium, Heavy)

Improved model learning using domain-specific feature creation

6️⃣ Feature Selection

Applied feature selection techniques such as:

Correlation analysis

Feature importance from tree-based models

Removed multicollinear and low-impact features to improve performance

7️⃣ Encoding & Scaling

Encoded categorical features (cut, color, clarity) using:

Ordinal Encoding / One-Hot Encoding

Scaled numerical features using standardization for ML and ANN models

8️⃣ Model Building – Regression

Split data into training and testing sets

Built multiple regression models:

Linear Regression

Decision Tree

Random Forest

KNN

XGBoost

Built an ANN regression model using TensorFlow/Keras

Evaluated models using MAE, MSE, RMSE, and R²

Saved the best-performing model as a .pkl file

9️⃣ Model Building – Clustering

Performed K-Means clustering for market segmentation

Determined optimal clusters using:

Elbow Method

Silhouette Score

Applied PCA for dimensionality reduction and cluster visualization

Assigned meaningful cluster names based on characteristics

Saved the clustering model as a .pkl file

🔟 Streamlit Application Development

Developed an interactive Streamlit web app with:

Diamond price prediction module

Market segment (cluster) prediction module

Took user inputs for diamond attributes

Displayed predicted price (INR) and cluster category in real time

✅ Final Outcome

Accurate diamond price prediction system

Clear market segmentation for business insights

Deployed, user-friendly Streamlit application

End-to-end ML pipeline suitable for real-world retail and luxury analytics

If you want, I can also:

Make this ATS-optimized

Shorten it for resume

Convert it to README markdown with emojis

Add project architecture diagram text
