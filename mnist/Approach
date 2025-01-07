# MNIST Classification using Neural Network

## Dataset Loading and Preprocessing:
   - Dataset was loaded using TensorFlow. It has about 60,000 training images and 10,000 test images.
   - The images were flattened, normalized (helps NN converge faster) and labels were one-hot encoded (here it's vector of length 10 --> 0-9 numbers,
     each element represents a class)

## Model Architecture:
   - Input layer consists of 784 neurons (flattened image length).
   - This is a pretty simple neural network and it has two hidden layers. Each dense layer followed by Batch normalization, dropout and activation (ReLU) layers. 
   - Batch normalization is applied after dense and before activation layer. It ensures  inputs to the activation function are normalized, 
     which can help the network learn more effectively. 
   - Dropout is used to prevent overfitting. It randomly deactivates certain percent of neurons during training. 
   - Output has 10 neurons with softmax activation (since it's multiclass)
 
## Model Compilation:
   - **Optimizer**: **Adam optimizer** was chosen to handle sparse gradients and noisy data.
   - **Loss Function**: **Categorical cross-entropy** was used as the loss function because the problem is a multiclass classification task.
   - **Metrics**: Accuracy

## Training, Evaluation and Results:
   - The model was trained for **5 epochs** with a batch size of **32** and valuated using **test accuracy**. Later was saved in `.h5` format.
   - Accuracy: Train - 95.80% | Val - 97.35% | Test - 97.73%

## Choice of Parameters:
   - **Batch Size (32)**: Chosen to balance training speed and model performance.
   - **Epochs (5)**: A reasonable starting point for experimenting. Additional epochs could improve accuracy further but may lead to overfitting without regularization.
   - **Dropout Rate (0.2)**: Dropout was used to prevent overfitting, and 20% is a commonly used value.
   - **Adam Optimizer**: Selected due to its adaptive learning rate, making it suitable for a variety of neural networks.
