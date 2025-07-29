# Cat and Dog Image Classifier

## Author
Peter Faux

## Description
This project is my solution to the [Cat and Dog Image Classifier challenge by freeCodeCamp](https://www.freecodecamp.org/learn/machine-learning-with-python/machine-learning-with-python-projects/cat-and-dog-image-classifier).

The task was to create a convolutional neural network (CNN) that can distinguish between images of cats and dogs. I used TensorFlow and Keras to build, train, and evaluate the model. While the dataset and some starter code were provided by freeCodeCamp, all model design, training logic, and evaluation strategies were written by me.

## Requirements
- Python 3.x  
- TensorFlow 2.x  
- NumPy  
- Matplotlib  

To run this in Google Colab, no installation is needed—just upload the notebook and run all cells.

## Project Structure

| Section                     | Description                                                                                                                                         |
|----------------------------|-----------------------------------------------------------------------------------------------------------------------------------------------------|
| Data Loading (Provided)    | freeCodeCamp provided code to download and extract the Cats vs. Dogs dataset.                                                                      |
| Data Augmentation (Mine)   | I applied transformations like rotation, zoom, shear, and horizontal flip to improve generalization.                                               |
| Data Generators (Mine)     | Created training, validation, and test generators using `ImageDataGenerator`.                                                                     |
| CNN Architecture (Mine)    | Built a 5-layer convolutional neural network with dropout and ReLU activations for binary classification.                                          |
| Training (Mine)            | Compiled the model with the Adam optimizer and used early stopping to prevent overfitting.                                                         |
| Evaluation Logic (Provided)| freeCodeCamp provided logic to compare predictions to a set of answers and determine if the model passes the challenge threshold (≥ 63% accuracy). |
| Visualization (Mixed)      | Used both provided and custom visualizations to show training progress and preview augmented images.                                                |

## How to Use

1. Open the notebook in [Google Colab](https://colab.research.google.com/).
2. Run each cell sequentially.
3. The final model will output its performance and indicate whether it passed the challenge threshold.

## How It Works

- **Image Preprocessing**: Normalizes pixel values and applies transformations to the training set.
- **Model Architecture**: A sequential CNN with multiple convolutional and pooling layers, followed by dense layers and dropout.
- **Training Process**: Uses binary crossentropy as the loss function and tracks validation loss to apply early stopping.
- **Evaluation**: Generates predictions on a test set and compares them to known labels to determine accuracy.

## License
This project follows the educational licensing and usage policies outlined by [freeCodeCamp](https://www.freecodecamp.org/news/terms-of-service/). Code written by me is shared for educational and portfolio use only.
