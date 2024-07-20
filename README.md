# Car Sales Prediction Project

## Project Overview
This project aims to predict the car purchase amount based on several customer features using a neural network model. The project involves data preprocessing, exploratory data analysis, model building, and evaluation.

## Libraries and Tools Used
- **Python Libraries**: 
  - `numpy`: For numerical computations.
  - `pandas`: For data manipulation and analysis.
  - `matplotlib` and `seaborn`: For data visualization.
  - `tensorflow` and `keras`: For building and training the neural network model.
  - `sklearn`: For preprocessing and model evaluation.

## Data Preprocessing
1. **Loading the Dataset**: The dataset is loaded from a CSV file using pandas.
2. **Dataset Overview**: The dataset contains 500 rows and 9 columns, which include customer details and the car purchase amount.
3. **Handling Missing Values**: Checked for missing values and found none.
4. **Handling Duplicate Values**: Checked for duplicate entries and found none.
5. **Dropping Unnecessary Columns**: Removed non-essential columns like `customer name` and `customer e-mail` to focus on relevant features.
6. **Label Encoding**: Encoded the `country` column into numerical values using `LabelEncoder`.

## Data Exploration
1. **Descriptive Statistics**: Used `describe()` to get an overview of the dataset.
2. **Correlation Analysis**: Created a heatmap to visualize correlations between features.
3. **Pairplot and Boxplot**: Visualized the distribution and relationships of features using pairplot and boxplot.
4. **Histograms and Countplots**: Explored the distribution of the car purchase amount and the gender distribution.

## Feature Engineering
- **Dependent Variable**: `car purchase amount`
- **Independent Variables**: `age`, `annual salary`, `credit card debt`, `net worth`, `country_encoded`, and `gender`

## Data Splitting
- Split the dataset into training (80%) and testing (20%) sets using `train_test_split`.

## Feature Scaling
- Applied `StandardScaler` to standardize the features for better performance of the neural network.

## Model Building
- **Architecture**: Built a neural network model with three layers using `keras`:
  - Input layer with 6 units.
  - Two hidden layers with 32 units each and ReLU activation.
  - Output layer with 1 unit and linear activation.
- **Compilation**: Compiled the model using the Adam optimizer and mean squared error loss function.
- **Training**: Trained the model for 100 epochs with a batch size of 32 and a validation split of 0.1.

## Model Evaluation
- Evaluated the model on the test set to obtain the mean squared error.

## Results
- The training and validation loss decreased consistently, indicating the model's learning progress.
- The final mean squared error on the test data was reported, showcasing the model's prediction performance.

## Conclusion
This project demonstrates the process of predicting car purchase amounts using a neural network. The steps include data preprocessing, exploratory data analysis, feature engineering, model building, and evaluation. The model can be further improved by tuning hyperparameters, trying different architectures, or using more advanced techniques.
