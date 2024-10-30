# Fashion MNIST with Convolutional Neural Networks (CNNs)

This project implements a Convolutional Neural Network (CNN) for classifying images from the Fashion MNIST dataset, which consists of 60,000 grayscale images of clothing items.

## Model Architecture

The CNN model, defined in the `BasicCNN` class, features:

- **Convolutional Layers**: 
  - **Conv Layer 1**: 1 input channel, 32 output channels, kernel size 3x3. 
  - **Conv Layer 2**: 32 input channels, 64 output channels, kernel size 3x3.
  
- **Pooling Layers**: Max pooling layers are used to down-sample feature maps.

- **Fully Connected Layers**: 
  - **FC Layer 1**: 128 neurons.
  - **FC Layer 2**: 10 neurons (for classification).

- **Activation Function**: ReLU is used for non-linearity, and softmax is applied to the output for classification.

## Training and Validation

The model is trained using PyTorch with `nn.CrossEntropyLoss` for loss calculation. Data augmentation techniques can be applied to enhance model performance.

## Results

After training, the model achieved the following results:
- **Overall Validation Loss**: 0.5887
- **Overall Validation Accuracy**: 91.54%

## Usage

1. Clone the repository.
2. Install required libraries (e.g., PyTorch).
3. Run the training script to train the model on the Fashion MNIST dataset.
4. Evaluate the model using the provided validation function.

## License

This project is licensed under the MIT License. Contributions and feedback are welcome!
