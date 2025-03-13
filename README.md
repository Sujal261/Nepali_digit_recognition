## Nepali Letter Recognition

This project aims to develop a machine learning model for recognizing handwritten Nepali letters using Convolutional Neural Networks (CNNs). The model has been trained and tested on a dataset of handwritten Nepali letters, demonstrating high accuracy and efficient recognition capabilities.

### Key Features:
- **Handwritten Nepali Letter Recognition**: Accurately recognizes letters written in Nepali.
- **Deep Learning Model**: Built using Convolutional Neural Networks (CNN) for image classification.
- **High Accuracy**: Achieves high accuracy in training and testing, showing its effectiveness for practical applications.
- **Batch Training**: The model is trained in batches, ensuring better optimization and faster convergence.

### Model Architecture:

The model is built using a CNN-based architecture to extract features from images and classify the Nepali letters. The architecture consists of:

- **Input Layer**: Accepts grayscale images of Nepali letters with a shape of 1x28x28 pixels.
- **Convolutional Layers**: 
  - First convolutional layer with a kernel size of 3x3, stride of 1, and padding of 1 to maintain spatial dimensions.
  - Second convolutional layer with the same kernel size, stride, and padding to further extract features.
- **ReLU Activation**: Applied after each convolutional layer to introduce non-linearity.
- **Max Pooling Layer**: Reduces spatial dimensions using a 2x2 kernel to down-sample the feature maps.
- **Fully Connected Layer**: A dense layer that outputs the final classification of the letters.
- **Output Layer**: Produces 46 output classes corresponding to Nepali letters.

#### Parameters:
- **Input Shape**: 1 (grayscale image with one channel)
- **Hidden Units**: 32 (number of feature maps in convolutional layers)
- **Output Shape**: 46 
- **Kernel Size**: 3x3 (used in both convolutional layers)
- **Stride**: 1 (the step size for the kernel)
- **Padding**: 1 (to preserve the spatial dimensions of the input image)
- **Max Pooling Kernel Size**: 2x2 (to reduce the feature map dimensions)
  
### Training and Testing Results:

 The result for final epoch is:

- **Final Epoch**: 
  - Train Loss: 0.0941
  - Train Accuracy: 97.08%
  - Test Loss: 0.2655
  - Test Accuracy: 93.21%

The model was trained using batches, which helped improve performance and generalization.

