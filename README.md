# NN_loss_landscape

This project visualizes the loss landscape of a Multi-Layer Perceptron (MLP) regressor by analyzing the error surface across various randomly initialized weight configurations.

## 🔍 What this project does:

- Initializes an `MLPRegressor` multiple times using weights drawn from a normal distribution.
- Computes the RMSE for each model instance on a fixed dataset.
- Applies PCA to reduce the high-dimensional weight space to 2D.
- Uses interpolation to smooth the scattered RMSE values over a grid.
- Generates interactive 3D surface and contour plots to visualize the loss/error landscape in the reduced space.

## 📦 Key Libraries Used:

- `scikit-learn` (MLPRegressor, PCA)
- `scipy` (griddata for interpolation)
- `plotly` (for interactive 3D and contour plotting)
- `numpy`, `pandas`

## 🎯 Purpose:

- The aim is to provide an educational example to better understand the structure of the MLP loss surface.
- Demonstrates how different random initializations can affect the model performance and convergence behavior.
