# 🧠 MNIST Handwritten Digit Classification using Deep Learning

A deep learning project that classifies handwritten digits (0–9) using the MNIST dataset. This project explores and compares three neural network approaches: a simple Perceptron-style model, an Artificial Neural Network (ANN), and a Convolutional Neural Network (CNN).

Built as my first CNN project, it helped me understand image preprocessing, neural network architectures, model evaluation, and computer vision fundamentals.

## 🎯 Project Objective

The objective is to train deep learning models to recognize handwritten digits from grayscale images of size 28 × 28 pixels and compare their classification performance.

## 📊 Model Performance

| Model | Test Accuracy |
|---|---:|
| Perceptron-style Model | 89.92% |
| Artificial Neural Network (ANN) | 98.86% |
| Convolutional Neural Network (CNN) | **99.50%** |

The CNN achieved the highest test accuracy among the three models in this experiment.

## 🛠️ Tech Stack

- **Programming Language:** Python
- **Data Processing:** NumPy, Pandas
- **Visualization:** Matplotlib, Seaborn
- **Deep Learning:** TensorFlow, Keras
- **Model Evaluation:** Scikit-learn
- **Dataset:** MNIST Handwritten Digits

## 📂 Project Workflow

1. **Data Loading:** Loaded the training and test datasets from CSV files.
2. **Data Inspection:** Checked dataset dimensions, column information, and missing values.
3. **Preprocessing:** Separated image pixels from labels and normalized pixel values to the range 0–1.
4. **Image Reshaping:** Reshaped images into 28 × 28 format for the basic models and 28 × 28 × 1 format for the CNN.
5. **Label Encoding:** Converted digit labels into one-hot encoded vectors.
6. **Model Building:** Developed and trained Perceptron-style, ANN, and CNN models.
7. **Model Evaluation:** Compared test accuracy and visualized training/validation accuracy and loss.
8. **Error Analysis:** Used a confusion matrix to examine the CNN's predictions.
9. **Prediction Visualization:** Compared predicted digits with actual labels.

## 🧩 Models Implemented

### 1. Perceptron-Style Model

- Flatten layer to convert image pixels into a feature vector.
- Dense output layer with 10 neurons.
- Softmax activation for multiclass classification.
- SGD optimizer and categorical cross-entropy loss.

### 2. Artificial Neural Network (ANN)

- Flatten input layer.
- Two hidden Dense layers with 128 and 64 neurons.
- ReLU activation in hidden layers.
- Softmax output layer with 10 classes.
- Adam optimizer and categorical cross-entropy loss.

### 3. Convolutional Neural Network (CNN)

- Two convolutional layers with 32 and 64 filters.
- ReLU activation for feature extraction.
- MaxPooling layers to reduce spatial dimensions.
- Flatten layer to prepare features for classification.
- Dense layer with 128 neurons.
- Dropout layer with a rate of 0.5 to help reduce overfitting.
- Softmax output layer for classifying digits from 0 to 9.

## 📈 Visualizations

The project includes:

- Training vs. validation accuracy plots.
- Training vs. validation loss plots.
- Validation accuracy comparison across models.
- CNN confusion matrix.
- Side-by-side comparison of actual and predicted digits.
- Final test accuracy comparison chart.

## 💡 Key Learnings

Through this project, I gained practical experience in:

- Understanding the difference between basic neural networks, ANNs, and CNNs.
- Preparing image data for deep learning.
- Building and training models with TensorFlow and Keras.
- Understanding convolution, pooling, flattening, and dropout.
- Evaluating classification models using accuracy and confusion matrices.
- Visualizing model performance and comparing architectures.

## 🚀 Getting Started

### Prerequisites

Make sure Python is installed on your system.

### 1. Clone the repository

```bash
git clone https://github.com/YOUR-USERNAME/MNIST-Handwritten-Digit-Classification.git
cd MNIST-Handwritten-Digit-Classification
```

Replace `YOUR-USERNAME` with your GitHub username.

### 2. Install dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn tensorflow jupyter
```

### 3. Prepare the dataset

Place `mnist_train.csv` and `mnist_test.csv` in the project directory.

The notebook expects the files to be available at:

```text
mnist_train.csv
mnist_test.csv
```

### 4. Run the notebook

Launch Jupyter Notebook:

```bash
jupyter notebook
```

Open the project notebook and run the cells sequentially.

## 📁 Suggested Project Structure

```text
MNIST-Handwritten-Digit-Classification/
│
├── MNIST_Handwritten_Digit_Classification.ipynb
├── mnist_train.csv
├── mnist_test.csv
├── README.md
└── requirements.txt
```

The dataset files are optional in the repository if you prefer to download them separately or provide a dataset source link.

## 🔮 Future Improvements

- Experiment with data augmentation.
- Add precision, recall, and F1-score comparisons.
- Analyze incorrectly classified images.
- Tune hyperparameters and experiment with different CNN architectures.
- Build an interactive web application for handwritten digit prediction.

## 👩‍💻 Author

**Vibhasha Suthar**

Aspiring Data Scientist | Machine Learning & Deep Learning Enthusiast

- GitHub: https://github.com/vibhashasuthar0712
- LinkedIn: https://linkedin.com/in/vibhasha-suthar-280b51351/

## ⭐ Acknowledgements

The MNIST handwritten digit dataset is a widely used benchmark for learning and experimenting with image classification and computer vision.

If you find this project useful, feel free to ⭐ the repository!
