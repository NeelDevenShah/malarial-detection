# malarial-detection
 Malaria detection using the cell images taken under microscope  
 
 The specific architecture defined in the code consists of multiple convolutional layers followed by max-pooling layers, a flatten layer, and two dense (fully connected) layers for classification. Here's a summary of the architecture:

Convolutional Layer: It applies 32 filters of size (3, 3) to the input image, with a ReLU activation function. This layer aims to extract 32 different features from the input images.

Max Pooling Layer: It performs max pooling with a pool size of (2, 2), reducing the spatial dimensions and making the model more efficient.

Convolutional Layer: Similar to the first convolutional layer, but with 64 filters of size (3, 3) and ReLU activation.

Max Pooling Layer: Another max pooling layer with a pool size of (2, 2).

Convolutional Layer: Similar to the previous layers, but with 128 filters of size (3, 3) and ReLU activation.

Max Pooling Layer: Another max pooling layer with a pool size of (2, 2).

Flatten Layer: This layer flattens the 3D output from the previous layer into a 1D vector, preparing it for the fully connected layers.

Dense Layer: A fully connected layer with 64 neurons and a ReLU activation function. It learns more complex patterns from the flattened features.

Dense Layer (Output Layer): The final fully connected layer with 1 neuron and a sigmoid activation function. It produces a probability output between 0 and 1, representing the likelihood of the input belonging to one of the classes (binary classification).

Overall, this architecture is relatively simple but can be effective for simple image classification tasks. For more complex tasks or larger datasets, more sophisticated architectures such as VGG, ResNet, or Inception may be employed.
