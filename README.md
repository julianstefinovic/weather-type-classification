# Weather Type Prediction using a Feed-forward Neural Network

A simple project demonstrating how to build and train a neural network to predict weather types (e.g., Rainy, Cloudy, Sunny, Snowy) based on atmospheric conditions like temperature, humidity, wind speed, and more. The process includes data preprocessing, model training, evaluation, and visualization. This project contains AI-generated code.

The project uses this [Dataset](https://www.kaggle.com/datasets/nikhil7280/weather-type-classification/data).

---

## **Steps Overview**

### **1. Data Preprocessing**
- **Data Loading**: The dataset is loaded from a CSV file.
- **Cleaning**: Certain columns like `'Cloud Cover'` are removed, in order to include only data from basic sensor measurements.
- **Normalization**: Numerical features are scaled using `MinMaxScaler`.
- **Splitting**: The data is split into training, validation, and test sets.

---

### **2. Model Architecture**
A simple feedforward neural network is built with three fully connected layers and ReLU activation functions. The model is designed to classify weather types based on the input features.

---

### **3. Training and Evaluation**
- **Training**: The model is trained using the Adam optimizer and CrossEntropyLoss. Training and validation accuracies are tracked over 2000 epochs.
- **Evaluation**: The model's performance is evaluated on the test set, and the final test accuracy is reported.

---

### **4. Visualization**
- **Accuracy Plot**: Training and validation accuracies are plotted over epochs to monitor learning progress.
- **Confusion Matrix**: A Confusion Matrix is used to visualize the model's performance across different weather types.
- **t-SNE Plot**: The last layer's output is reduced to 2D using t-SNE for visualizing the distribution of weather types in the feature space.
- **Interactive**: Open up the Jupyter Notebook to see which data points were misclassified, and to see the associated data vector

---

## **Results**
The model achieves a final test accuracy of around `81.4%` on the validation set.

---

## **Conclusion**
This project showcases the end-to-end process of building a neural network for weather prediction. It highlights the importance of data preprocessing, model training, and visualization in machine learning workflows. Future improvements could include experimenting with different architectures or adding more features.

---

Feel free to explore the code and adapt it to your own datasets! For questions or suggestions, open an issue or submit a pull request.
