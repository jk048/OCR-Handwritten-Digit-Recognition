# OCR_Final: Handwritten Digit Recognition Using CNN (MNIST)

This project is a complete solution for recognizing handwritten digits using a Convolutional Neural Network (CNN) trained on the MNIST dataset. It includes model training, evaluation, and a user interface for predicting custom images.

---

## Features

- **CNN Model Training**: Trains a CNN on the MNIST dataset for digit classification.
- **Model Persistence**: Automatically saves and loads the trained model to avoid retraining.
- **Performance Visualization**: Plots training and validation accuracy/loss.
- **Test Evaluation**: Evaluates the model on the MNIST test set.
- **Custom Image Prediction**: Upload your own digit images (e.g., scanned or photographed) and get predictions.
- **Interactive Visualization**: Shows uploaded images with predicted labels.

---

## Requirements

- Python 3.x
- TensorFlow (tested with TensorFlow 2.x)
- numpy
- matplotlib
- scikit-learn
- OpenCV (`cv2`)
- Google Colab (for image upload widget; can be adapted for local use)

---
### A. Model Training and Evaluation

1. **Train the Model**  
   - Loads and preprocesses the MNIST dataset.
   - Builds and trains a CNN model (or loads a saved model if it exists).
   - Plots training and validation metrics.
   - Evaluates accuracy on the test set.

2. **Model Architecture**
   - 3 × Conv2D layers (32, 64, 64 filters)
   - 2 × MaxPooling2D layers
   - Flatten + Dense (64 units, ReLU)
   - Output Dense (10 units, Softmax)
   - Optimizer: SGD (learning rate 0.01)
   - Loss: Sparse Categorical Crossentropy

3. **Sample Output**
   - Test accuracy: ~97.7%
   - Visualizes predictions on sample test images.

### B. Predicting Custom Images

1. **Upload Images**  
   - Upload one or more images (`.jpg`, `.png`) of handwritten digits.
   - Images are preprocessed: grayscale, resized to 28×28, inverted (white digit on black), normalized.

2. **Prediction**  
   - The model predicts the digit and displays the image with the result.
## Example Results

- **Test Accuracy**: ~97.7% on MNIST test set.
- **Prediction**: Custom images are displayed with predicted digit labels.

---

## License

This project is released under the MIT License.

---

## Acknowledgments

- [MNIST Dataset](http://yann.lecun.com/exdb/mnist/)
- TensorFlow/Keras documentation
- Google Colab for interactive features

---

Feel free to use, modify, and extend this project for your digit recognition or OCR experiments!

