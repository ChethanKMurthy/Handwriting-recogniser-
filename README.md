```markdown
# Handwritten Digit Recognition using TensorFlow ✍️🔢

This project demonstrates how to build and train a simple neural network model for handwritten digit recognition using TensorFlow and Keras on the MNIST dataset.

## Requirements
- Python 3.x
- TensorFlow
- NumPy
- Joblib

Install the required libraries using pip:
```bash
pip install tensorflow numpy joblib
```

## Usage
1. Clone the repository or download the script.
2. Run the script `handwritten_digit_recognition.py`.

## Description
This script loads the MNIST dataset, builds a simple neural network model, trains it on the training data, and saves the trained model.

### Steps:
1. **Import Libraries**:
   - TensorFlow is imported as `tf`.
   - Specific modules from TensorFlow are imported to load the dataset and build the model.
   - `joblib` is imported to save the trained model.

2. **Load the Dataset**:
   - The MNIST dataset is loaded using `mnist.load_data()`.
   - The dataset is then preprocessed by scaling the pixel values to the range [0, 1].

3. **Build the Neural Network Model**:
   - A simple sequential model is created using `Sequential()`.
   - It consists of a Flatten layer as input, followed by two Dense layers.
   - The first Dense layer has 128 units with ReLU activation.
   - The output layer has 10 units (one for each digit) with softmax activation.

4. **Compile the Model**:
   - The model is compiled with 'adam' optimizer and 'sparse_categorical_crossentropy' loss function.
   - Accuracy is used as a metric.

5. **Train the Model**:
   - The model is trained using `model.fit()` on the training data.
   - Training is performed for 5 epochs.

6. **Save the Model**:
   - The trained model is saved as `mnist_model.h5` using `model.save()`.

## Dataset
The MNIST dataset is a widely used dataset for handwritten digit classification. It contains 60,000 training images and 10,000 testing images of handwritten digits (0 to 9), each of size 28x28 pixels.

## Credits
- This project uses the MNIST dataset provided by TensorFlow/Keras.
- Inspired by TensorFlow documentation and tutorials.

Feel free to modify and use this code for your own projects! 🚀
```

Now it's all set with relevant emojis! ✨
