# Plant-Classification-Model-using-CNN

Dataset : "https://flavia.sourceforge.net/"

Methodology

In this project, we developed a deep learning model to classify images of leaves using the Convolutional Neural Network (CNN) approach.
We started by loading the dataset located in Google Drive. All images were processed and normalized to have the same dimensions of 64x64 pixels and were converted to grayscale to reduce computational load.
The data was split into three parts: 60% for training, 20% for validation, and 20% for testing. This was done to ensure the model could be trained on a substantial portion of the data and validated and tested on unseen data.
Our Convolutional Neural Network (CNN) model uses two sets of convolutional and max-pooling layers to extract and simplify image features. A dropout layer was added for robustness and to prevent overfitting. The data was then flattened into a 1D array, passed through two dense layers for classification. Finally, a softmax activation function in the output layer predicts the probability distribution over the 32 classes.
The model was compiled with the Adam optimizer and sparse categorical cross-entropy as the loss function. It was trained for five epochs.

Results

The model achieved an accuracy of 70.2% on the test set, with a precision of 73.3%, a recall of 70.2%, and a F1-score of 68.9%. The confusion matrix shows that the model performs well on most classes, but struggles with some.

Limitations and Improvements

The model might benefit from more training data, especially for the classes it struggles with.
Future improvements could involve:
Augmenting the dataset: This can include techniques like rotating, zooming, or shifting the input images to create a more diverse dataset and prevent overfitting.
Adding regularization techniques: This could be L1/L2 regularization to make the model more robust.
Complex Model Architecture: Depending upon the diversity and complexity of the dataset, a more sophisticated architecture could be employed.
Fine-tuning the model architecture, using a pre-trained model, or implementing an ensemble of models could also potentially improve performance.
Cross-validation: This can help in assessing how the model's results would generalize to an independent dataset.
In conclusion, while the model exhibits outstanding performance on the current dataset, further testing and possibly enhancements are required to ensure its robustness and ability to generalize to other unseen and diverse sets of leaf images.

