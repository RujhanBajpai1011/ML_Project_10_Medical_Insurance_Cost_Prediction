# 🏥 Medical Insurance Cost Prediction

This project aims to predict individual medical insurance costs based on various demographic and health factors. It uses a Linear Regression model, a fundamental machine learning algorithm for predicting continuous values. The project includes data analysis, visualization, preprocessing, model training, and evaluation.

## **📊 Dataset**

The dataset used is insurance.csv. It contains information about individuals, including:

* **age**: Age of the primary beneficiary.
* **sex**: Gender (male/female).
* **bmi**: Body Mass Index, providing an understanding of body, weight, and height.
* **children**: Number of children covered by health insurance.
* **smoker**: Whether the beneficiary is a smoker or not.
* **region**: The beneficiary's residential area in the US (northeast, southeast, southwest, northwest).
* **charges**: Individual medical costs billed by health insurance (the target variable).

## **✨ Features**

* **Data Loading and Initial Exploration**: Loads the insurance.csv dataset into a pandas DataFrame and performs initial checks such as displaying the first few rows, checking its shape (number of rows and columns), and getting a summary of its structure and data types.

* **Missing Value Check**: Confirms the absence of missing values across all columns, ensuring data completeness for analysis.

* **Statistical Summary**: Provides descriptive statistics for numerical features, offering insights into their central tendency, dispersion, and shape.

* **Data Distribution Visualization**: Utilizes seaborn to visualize the distribution of key numerical features like age, bmi, and charges using distribution plots.

* **Categorical Feature Distribution**: Employs count plots to show the distribution of categorical features such as sex, smoker, and region, making it easy to see the counts for each category.

* **Categorical to Numerical Conversion**: Transforms categorical columns (sex, smoker, region) into numerical representations using label encoding to prepare them for the machine learning model.

* **Feature and Target Separation**: Splits the processed dataset into features (X) and the target variable (Y), where charges is the variable to be predicted.

* **Data Splitting**: Divides the dataset into training and testing sets (80% training, 20% testing) to train and evaluate the model effectively.

* **Linear Regression Model Training**: Trains a Linear Regression model on the training data.

* **Model Evaluation**: Assesses the model's performance using R-squared error on both the training and test datasets.

* **Predictive System**: Demonstrates how to use the trained model to predict the insurance cost for a new set of input data.

## **🛠️ Technologies Used**

* **Python**

* **pandas**: For robust data manipulation and analysis.

* **numpy**: For advanced numerical operations, especially with arrays.

* **matplotlib.pyplot**: For creating static, interactive, and animated visualizations.

* **seaborn**: For producing attractive and informative statistical graphics.

* **scikit-learn**: For machine learning functionalities, including:
  * train_test_split: To divide the dataset.
  * LinearRegression: The core regression algorithm used.
  * metrics: For calculating evaluation metrics like R-squared error.

## **📦 Requirements**

To run this project, you will need the following Python libraries:

* pandas
* numpy
* matplotlib
* seaborn
* scikit-learn

## **🚀 Getting Started**

To get this project up and running on your local machine, follow these simple steps.

### **Installation**

1. **Clone the repository (if applicable):**

```
git clone <repository_url>
cd <repository_name>
```

2. **Install the required Python packages:**

```
pip install pandas numpy matplotlib seaborn scikit-learn
```

### **Usage**

1. **Place the dataset**: Ensure the insurance.csv file is located in the same directory as the Jupyter notebook (Medical_Insurance_Cost_Prediction.ipynb).

2. **Run the Jupyter Notebook**: Open and execute all the cells in the Medical_Insurance_Cost_Prediction.ipynb notebook in a Jupyter environment (e.g., Jupyter Lab, Jupyter Notebook, Google Colab).

The notebook will:

* Load and preprocess the insurance data.
* Perform exploratory data analysis and visualize distributions.
* Train the Linear Regression model.
* Output the R-squared error scores for both training and test data.
* Demonstrate a prediction for a sample input, estimating the insurance cost.

## **📈 Results**

The notebook provides the R-squared error for the Linear Regression model, which indicates the proportion of variance in the dependent variable that can be predicted from the independent variables. Higher R-squared values suggest a better fit.

* **R-squared Value (Training Data)**: Approximately 0.7515
* **R-squared Value (Test Data)**: Approximately 0.7447

These results show that the model performs consistently on both seen and unseen data, demonstrating its ability to generalize. The predicted insurance cost for a sample input is also displayed.

## **🧑‍💻 Contributing**

Contributions are most welcome! If you have suggestions for improving the model, adding new features, or enhancing the analysis, please feel free to:

1. Fork the repository.
2. Create your feature branch (git checkout -b feature/AmazingFeature).
3. Commit your changes (git commit -m 'Add some AmazingFeature').
4. Push to the branch (git push origin feature/AmazingFeature).
5. Open a Pull Request.
