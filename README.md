# MNIST Handwritten Digit Classification

## Overview
This project uses a deep learning model built with TensorFlow and Keras to recognize handwritten digits from 0 to 9 using the MNIST dataset. The model is trained using a fully connected (Dense) neural network to classify grayscale handwritten digit images.

## Project Objectives
- Load and explore the MNIST dataset.
- Preprocess and normalize image data.
- Build a Sequential Dense Neural Network.
- Train the model for 5 epochs.
- Evaluate model performance using test data.
- Visualize training accuracy and loss.
- Save the trained model in H5 format.
- Perform digit predictions using the trained model.

## Dataset
The MNIST dataset contains handwritten digit images.

- Training images: 60,000
- Testing images: 10,000
- Image size: 28 × 28 pixels
- Color format: Grayscale
- Classes: 10 (digits 0–9)

## Technologies Used
- Python
- TensorFlow
- Keras
- NumPy
- Matplotlib
- Jupyter Notebook / Google Colab

## Model Architecture
The model uses a Sequential neural network with the following layers:

1. Input Layer — accepts 28 × 28 images
2. Flatten Layer — converts images into a 1D feature vector
3. Dense Layer — 512 neurons, ReLU activation
4. Dropout — 20%
5. Dense Layer — 256 neurons, ReLU activation
6. Dropout — 20%
7. Output Layer — 10 neurons, Softmax activation

This project uses a fully connected neural network without convolutional layers.

## Model Configuration
- Optimizer: Adam
- Loss Function: Categorical Crossentropy
- Evaluation Metric: Accuracy
- Epochs: 5
- Batch Size: 128
- Validation Split: 10%

## Project Workflow
1. Import required libraries.
2. Load the MNIST dataset.
3. Normalize pixel values between 0 and 1.
4. Convert digit labels into one-hot encoding.
5. Build the neural network model.
6. Compile the model.
7. Train the model.
8. Evaluate the model on test data.
9. Plot accuracy and loss curves.
10. Save the trained model.
11. Load the saved model and test predictions.

## Expected Performance
The model is expected to achieve approximately 97–98% test accuracy under typical training conditions. Actual performance may vary depending on the execution environment.

## How to Run

### Option 1: Google Colab
1. Download the notebook from this repository.
2. Open [Google Colab](https://colab.research.google.com/).
3. Upload the `.ipynb` notebook.
4. Select **Runtime → Run all**.
5. Wait for training and evaluation to finish.

### Option 2: Jupyter Notebook
Install the required packages:

```bash
pip install tensorflow numpy matplotlib notebook
```

Launch Jupyter:

```bash
jupyter notebook
```

Open the notebook and run all cells sequentially.

## Files Included
- `MNIST_Digit_Classification.ipynb` — Complete project notebook with preprocessing, training, evaluation, visualization, and prediction.
- `mnist_dense_model.h5` — Saved trained model generated after execution.

## Results
The project outputs:
- Training and validation accuracy
- Training and validation loss
- Test accuracy and test loss
- Digit prediction results
- Saved trained neural network model

## Future Improvements
- Experiment with different numbers of hidden layers and neurons.
- Tune learning rate and batch size.
- Improve generalization with additional regularization.
- Compare the Dense Neural Network with a Convolutional Neural Network (CNN).

## Author
## Purva Ghate ##
Created as a Deep Learning / Machine Learning project for handwritten digit classification.

## License
This project is intended for educational and learning purposes.
