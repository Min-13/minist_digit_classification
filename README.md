🧠 MNIST Digit Classification with TensorFlow
Overview

This project implements a feedforward neural network using TensorFlow/Keras to classify handwritten digits from the MNIST dataset. The model is trained to recognize digits (0–9) from 28×28 grayscale images.

📊 Dataset

60,000 training images

10,000 test images

Each image: 28×28 grayscale

Labels: Integers from 0 to 9

🏗 Model Architecture

Input (28×28 image)
↓
Flatten Layer (784 features)
↓
Dense Layer (128 neurons, ReLU)
↓
Dropout (0.2)
↓
Dense Output Layer (10 logits)

🔬 Training Details

Loss: Sparse Categorical Crossentropy (from_logits=True)

Optimizer: Adam (learning rate = 0.01)

Epochs: 10

Metric: Accuracy

🎯 Key Design Decisions

Normalization improves gradient stability.

Dropout reduces overfitting.

Logits instead of softmax in output improves numerical stability during training.

Sparse loss avoids one-hot encoding labels.

📈 Results

The model achieves high accuracy on the MNIST test dataset after 10 epochs of training.
