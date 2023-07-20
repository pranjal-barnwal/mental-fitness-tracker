# Mental Fitness Tracker ML Model

<img src="https://i.pinimg.com/originals/bf/ce/69/bfce69e525225d1fdc96caa204e2d9e7.gif" />

## GLIMPSES

**Pickle Model:** [Mental Fitness Tracker Pickle Model](https://drive.google.com/file/d/1WzmfkdzvgSOm7uQQbVakmaEjm9a4rI6e/view?usp=drive_link)

**Presentation:** [Mental Fitness Tracker Presentation](https://docs.google.com/presentation/d/1OOdo-VLhvjbUscd1-qMpY6PDNPYckFYD/edit?usp=sharing&ouid=108712502165030352442&rtpof=true&sd=true)



Welcome to the repository of the Mental Fitness Tracker ML Model! Our project introduces a machine learning model to monitor mental fitness effectively. The Random Forest Regression algorithm powers this model, offering valuable insights into mental well-being based on input features.

## Table of Contents

- [About the Mental Fitness Tracker](#about-the-mental-fitness-tracker)
- [Key Features](#key-features)
- [Getting Started](#getting-started)
- [Model Evaluation](#model-evaluation)
- [Usage](#usage)
- [Contributing](#contributing)
- [Acknowledgments](#acknowledgments)
- [License](#license)

## About the Mental Fitness Tracker
The Mental Fitness Tracker ML Model evaluates and tracks mental well-being using the Random Forest Regression algorithm. The model analyzes input features and predicts mental fitness levels based on the provided data.

## Key Features
- Utilizes Random Forest Regression for accurate prediction of mental fitness.
- Provides model evaluation metrics such as Mean Squared Error (MSE), Root Mean Squared Error (RMSE), and R-Squared (R2) score.
- Offers a pickled model for easy usage and integration into other applications.
- Includes a presentation highlighting the project details and methodology.

## Getting Started

To get started with the Mental Fitness Tracker ML Model, follow these instructions:

1. Clone the repository:
   ```sh
   git clone https://github.com/pranjal-barnwal/mental-fitness-tracker
   ```

2. Install the required dependencies (such as scikit-learn) using the package manager of your choice.

3. Review the project structure, including the model code, presentation, and pickled model.

## Model Evaluation

The model is evaluated on both the training and testing datasets. The evaluation metrics are calculated using the Random Forest Regression model:

### Training Set Evaluation

```python
# Model evaluation for the training set
ytrain_pred = rf.predict(xtrain)
mse = mean_squared_error(ytrain, ytrain_pred)
rmse = np.sqrt(mean_squared_error(ytrain, ytrain_pred))
r2 = r2_score(ytrain, ytrain_pred)

print("The model performance for the training set")
print("--------------------------------------------")
print('MSE is {}'.format(mse))
print('RMSE is {}'.format(rmse))
print('R2 score is {}'.format(r2))
print("\n")
```

### Testing Set Evaluation

```python
# Model evaluation for the testing set
ytest_pred = rf.predict(xtest)
mse = mean_squared_error(ytest, ytest_pred)
rmse = np.sqrt(mean_squared_error(ytest, ytest_pred))
r2 = r2_score(ytest, ytest_pred)

print("The model performance for the testing set")
print("-------------------------------------------")
print('MSE is {}'.format(mse))
print('RMSE is {}'.format(rmse))
print('R2 score is {}'.format(r2))
```

## Usage

To use the Mental Fitness Tracker ML Model, follow these steps:

1. Load the pickled model from the provided Google Drive link: [Mental Fitness Tracker Pickle Model](https://drive.google.com/file/d/1WzmfkdzvgSOm7uQQbVakmaEjm9a4rI6e/view?usp=drive_link).
2. Prepare the input data according to the model's requirements.
3. Utilize the model's predict method to obtain mental fitness predictions based on the input data.

### Sample Input and Output

```python
# Sample input
ata = [[0, 1991, 0.228120, 0.719953, 0.126395, 4.821965, 0.447112, 5.116306, 0.444250]]

# Predict the mental fitness quotient
ress = rf.predict(ata)

print("Your Mental Fitness Quotient Is:", ress)
```

## Contributing

Contributions are welcome and greatly appreciated! If you have any suggestions, ideas, or improvements, please submit a pull request. Feel free to open an issue for any bug reports or feature requests.

## Acknowledgments

I would like to express my gratitude to the open-source community and the authors of the scikit-learn library for providing the tools and resources necessary for this project.

## License

This project is licensed under the [MIT License](LICENSE). Feel free to use and modify the code for your own purposes.

---

Thank you for your interest in the Mental Fitness Tracker ML Model! I hope this model helps improve mental well-being tracking and understanding. If you have any questions or need further assistance, please don't hesitate to reach out.

Happy tracking!

[Pranjal Kumar]
