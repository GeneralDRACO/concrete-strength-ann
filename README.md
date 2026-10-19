# Concrete Compressive Strength Prediction Using ANN

## Project Overview
This project develops an Artificial Neural Network (ANN) to predict concrete compressive strength using concrete mixture proportions and curing age.

The model is implemented in Python using TensorFlow/Keras in a Jupyter Notebook.

## Dataset
The project uses the UCI Concrete Compressive Strength dataset.

- **Observations:** 1,030
- **Input features:** 8
- **Target:** Concrete compressive strength (MPa)

Input features include cement, blast furnace slag, fly ash, water, superplasticizer, coarse aggregate, fine aggregate, and curing age.

**Dataset source:** https://archive.ics.uci.edu/dataset/165/concrete+compressive+strength

## Methodology
1. Load and inspect the dataset.
2. Perform data-quality checks and exploratory analysis.
3. Split the data into training and testing sets.
4. Standardize input features using training-set statistics.
5. Train an ANN with two hidden layers using ReLU activation.
6. Evaluate the model on held-out test data.
7. Visualize actual versus predicted strength and training performance.

## Model Performance

| Metric | Test Result |
|---|---:|
| Mean Absolute Error (MAE) | 4.51 MPa |
| Root Mean Squared Error (RMSE) | 5.8 MPa |
| R² Score | 0.874 |

These results correspond to the current train-test split. Performance may differ on other datasets or splits.

## Technologies Used
- Python
- Pandas and NumPy
- Matplotlib
- Scikit-learn
- TensorFlow/Keras
- Google Colab

## How to Run
1. Open `Concrete_Strength_ANN.ipynb` in Google Colab or Jupyter Notebook.
2. Install any required libraries that are not already available.
3. Run the notebook cells in order.

## Limitations
The model is based on a specific dataset and has not necessarily been validated on independent concrete mixtures. Predictions are for educational and research purposes and do not replace laboratory testing or approved concrete mix-design procedures.
