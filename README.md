# medical_insurance


```markdown
# Insurance Cost Prediction

This project aims to predict insurance charges based on various features such as age, gender, BMI, smoking status, region, and the number of children using a Linear Regression model.

## Dataset

The dataset used for this project is `insurance.csv`, which contains the following columns:

- **age**: Age of the primary beneficiary
- **sex**: Gender of the primary beneficiary (male, female)
- **bmi**: Body Mass Index (BMI)
- **children**: Number of children covered by health insurance
- **smoker**: Smoking status (yes, no)
- **region**: Region of the beneficiary (southeast, southwest, northwest, northeast)
- **charges**: Medical costs billed by the insurance company

### Dataset Summary

- Total Rows: 1338
- Total Columns: 7

## Dependencies

This project requires the following libraries:

- `pandas`
- `numpy`
- `scikit-learn`
- `seaborn`
- `matplotlib`

You can install the required dependencies with the following command:

```bash
pip install pandas numpy scikit-learn seaborn matplotlib
```

## Exploratory Data Analysis (EDA)

We performed exploratory data analysis to understand the distribution and relationships between different features. Some visualizations include:

- Age distribution
- Sex distribution
- BMI distribution
- Number of children distribution
- Smoker status distribution
- Region distribution
- Charges distribution

## Preprocessing

We converted categorical variables (`sex`, `smoker`, `region`) into numerical values:

- `sex`: male → 0, female → 1
- `smoker`: yes → 0, no → 1
- `region`: southeast → 0, southwest → 1, northeast → 2, northwest → 3

## Model

We used a **Linear Regression** model to predict the `charges` based on the input features:

- Features: `age`, `sex`, `bmi`, `children`, `smoker`, `region`
- Target: `charges`

### Model Training

The dataset was split into training and testing sets:

- Training set: 80%
- Testing set: 20%

The model was trained using the training set, and the performance was evaluated on the testing set.

### Evaluation

The performance of the model was evaluated using the **R² Score**.

## Results

After training the Linear Regression model, we achieved the following results:

- R² Score on Training set: *`67%`*
- R² Score on Test set: *`66%`*

## Visualizations

We generated various plots to visualize the distribution of the dataset:

- Age Distribution
- BMI Distribution
- Charges Distribution
- Region and Smoker Distribution

## Usage

To run the code and reproduce the results, follow these steps:

1. Install the dependencies using the command provided above.
2. Load the dataset using `pandas`.
3. Perform exploratory data analysis (EDA).
4. Preprocess the data (encoding categorical variables).
5. Train the Linear Regression model using `scikit-learn`.
6. Evaluate the model on the testing set.



## License

This project is licensed under the MIT License.
