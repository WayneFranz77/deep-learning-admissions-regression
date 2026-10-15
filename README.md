# Deep Learning Regression with Admissions Data

## Project Overview

This project uses TensorFlow and Keras to develop a deep learning regression model that predicts a student's probability of admission to graduate school.

The model is trained on historical admissions data containing academic performance indicators, university ratings, letters of recommendation, statement of purpose scores, and research experience.

## Dataset

The dataset contains 500 graduate school applications with the following features:

- GRE Score
- TOEFL Score
- University Rating
- SOP
- LOR
- CGPA
- Research Experience

Target Variable:

- Chance of Admit

## Technologies Used

- Python
- Pandas
- NumPy
- TensorFlow
- Keras
- Scikit-Learn
- Matplotlib
- Seaborn

## Data Preparation

- Removed non-predictive identifier column (`Serial No.`)
- Standardised column names
- Split data into training and testing sets (80/20)
- Applied feature scaling using `StandardScaler`

## Model Architecture

```python
Dense(64, activation="relu")
Dense(32, activation="relu")
Dense(1, activation="linear")
```

## Results

- Training Samples: 400
- Testing Samples: 100
- R² Score: 0.7591

The model successfully explained approximately 75.9% of the variation in graduate school admission probability.

## Future Improvements

- Early Stopping
- Dropout Regularisation
- Hyperparameter Tuning
- Alternative Neural Network Architectures

## License

This project is licensed under the MIT License.