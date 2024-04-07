# Brain Tumor Classifier Using Convolutional Neural Networks (CNN)

This repository contains Python code for implementing a binary classification model to detect brain tumors from medical images using Convolutional Neural Networks (CNN). The model is evaluated on different activation functions and test-train splits to assess its performance.

# Requirements

    Python 3.x
    TensorFlow
    NumPy
    Pandas
    Matplotlib
    OpenCV

# Dataset

The dataset used for training and testing the model is available in the /kaggle/input/braintumour/BT directory. It consists of brain tumor images categorized into 'Tumor' and 'NoTumor' classes.

# Model Architecture

The CNN model architecture used for brain tumor classification is defined as follows:

    Input Layer: 200x200x3 (RGB image)
        Convolutional Layers:
            256 filters with 2x2 kernel and ReLU activation
            128 filters with 2x2 kernel and ReLU activation
            64 filters with 2x2 kernel and ReLU activation
            32 filters with 2x2 kernel and ReLU activation
        MaxPooling Layers: Applied after each convolutional layer
        Flatten Layer
        Dense Layers:
            512 neurons with ReLU activation
            Batch Normalization
            Dropout (0.1)
            512 neurons with ReLU activation
            Batch Normalization
            Dropout (0.2)
            512 neurons with ReLU activation
            Batch Normalization
        Output Layer: 1 neuron with Sigmoid activation

# Evaluation

The model is evaluated using various activation functions and different test-train splits. Performance metrics such as accuracy, loss, sensitivity, specificity, precision, and recall are calculated and plotted for analysis.

# Results

Confusion Matrix: A heatmap visualizing the true positive, true negative, false positive, and false negative predictions.
Blob Detection: OpenCV is used to detect and visualize blobs in the input images, indicating the presence of tumors.

# Conclusion

This project aims to provide a robust CNN-based classifier for the early detection of brain tumors.
