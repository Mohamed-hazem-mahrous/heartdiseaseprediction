# README for Notebook_team6.ipynb

This notebook contains code for analyzing and preprocessing the "heart" dataset. The dataset contains various features related to heart health and a target variable indicating the presence or absence of heart disease.

## Getting Started

To run the code in this notebook, you need to have the following dependencies installed:

- numpy
- pandas
- matplotlib
- seaborn
- scipy
- scikit-learn

You can install these dependencies using pip:


You also need to have Jupyter Notebook or JupyterLab installed to open and run the notebook.

## Dataset

The dataset used in this notebook is obtained from the following source:

[Heart Disease UCI](https://archive.ics.uci.edu/ml/datasets/heart+Disease)

The dataset contains the following columns:

- age: age of the patient (in years)
- sex: sex of the patient (1 = male, 0 = female)
- cp: chest pain type (1 = typical angina, 2 = atypical angina, 3 = non-anginal pain, 4 = asymptomatic)
- trestbps: resting blood pressure (in mm Hg)
- chol: serum cholesterol (in mg/dl)
- fbs: fasting blood sugar > 120 mg/dl (1 = true, 0 = false)
- restecg: resting electrocardiographic results (0 = normal, 1 = having ST-T wave abnormality, 2 = showing probable or definite left ventricular hypertrophy)
- thalach: maximum heart rate achieved
- exang: exercise-induced angina (1 = yes, 0 = no)
- oldpeak: ST depression induced by exercise relative to rest
- slope: the slope of the peak exercise ST segment (1 = upsloping, 2 = flat, 3 = downsloping)
- ca: number of major vessels (0-3) colored by fluoroscopy
- thal: 3 = normal, 6 = fixed defect, 7 = reversible defect
- target: presence of heart disease (1 = yes, 0 = no)

## Code Overview

1. Data Import and Exploration:
   - The necessary libraries (numpy, pandas, matplotlib, seaborn) are imported.
   - The dataset is read from a CSV file using the pandas `read_csv()` function.
   - The first 10 rows of the dataset are displayed to get a quick overview of the data.
   - The columns of the dataset are printed.

2. Data Preprocessing:
   - The dataset is divided into categorical and quantitative variables.
   - The z-score method is used to remove outliers from the dataset.
   - The interquartile range (IQR) method is also used to remove outliers.
   - The original data and the data without outliers are compared by calculating summary statistics and plotting histograms.
   - The columns are further divided into quantitative and categorical variables.

3. Data Analysis:
   - Measures of central tendency (mean, median, mode) are calculated for each column.
   - Measures of dispersion (standard deviation, variance, range, IQR) are calculated for each column.
   - The data is standardized by subtracting the mean and dividing by the standard deviation.
   - The dataset is split into training and testing subsets using the train_test_split function from scikit-learn.

4. Data Visualization:
   - Histograms are plotted for each feature to visualize the distributions.
   - The type of each distribution (Gaussian, exponential, uniform, etc.) is commented on.
   - Statistical tests (Shapiro-Wilk, D'Agostino-Pearson, Anderson-Darling) are performed to check for normality.

5. Conclusion:
   - The notebook provides an overview of the heart dataset and performs basic data analysis and preprocessing steps.
   - Further analysis and modeling can be performed based on the insights gained from this notebook.

## Usage

You can open the notebook using Jupyter Notebook or JupyterLab by running the following command in your terminal:

or


Once the notebook is open, you can run the code cells individually or use the "Run All" option to execute all cells sequentially.

## Contributing

Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.

