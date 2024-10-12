# Polynomial-Regression with Neural Networks (Keras)
This project implements a polynomial regression using a deep neural network (DNN) to model the relationship between time steps and position (y) in a dataset. The code uses TensorFlow and Keras to build and train the neural network. The dataset is preprocessed, normalized, and split into training and validation sets. The model’s performance is evaluated using metrics like Mean Absolute Error (MAE) and R² score. The results are visualized using Matplotlib.

1)Dataset

orbit.csv: The dataset used in the code, containing `time_steps` and `y` (position) columns.

2)Install need libraries

--> pip install pandas numpy scikit-learn tensorflow keras matplotlib


3)Project Structure

*Data Loading and Preprocessing*:
__________________________________

-The dataset is loaded from a CSV file (orbit.csv).
-Null values and data types are checked.
-The data distribution of time_steps and y are visualized using box plots and histograms.
-Skewness of the y variable is calculated.
-The dataset is normalized using the MinMaxScaler.

*Model*:
________

-A simple feedforward neural network (DNN) is created using Keras.
-The model consists of two hidden layers with 64 neurons each and ReLU activation.
-The output layer has one neuron for regression prediction.

*Training*:
___________

-The model is compiled using the Adam optimizer and mean_squared_error as the loss function.
-The model is trained for 100 epochs, and the training process is monitored by plotting the training and validation losses.

*Evaluation*:
_____________

-The model is evaluated on the validation set using MAE and R² metrics  (R² = 0.99).
-A scatter plot visualizes the actual vs predicted values of the validation set.
