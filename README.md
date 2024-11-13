3D Printer Error Detection: Nozzle Extrusion Classification
This project is focused on classifying 3D printer nozzle images to determine whether extrusion occurred or not, using the Attention-based Residual Convolutional Neural Network (ARCNN) model for image classification. The goal is to detect potential 3D printing errors based on nozzle images, which can indicate issues such as clogging, improper extrusion, or other failures.

Project Objectives
Classify Extrusion Occurrence: Predict whether extrusion occurred based on images of the 3D printer nozzle.
Model Development: Implement and train the ARCNN (Attention-based Residual Convolutional Neural Network) to classify images as either "extrusion occurred" or "no extrusion."
Data Preprocessing: Clean and prepare the image dataset for training, including resizing, normalization, and augmentation if necessary.
Model Training & Evaluation: Train the ARCNN model on the preprocessed dataset and evaluate it using metrics such as accuracy, precision, recall, and F1 score.
Prediction & Visualization: Make predictions on new nozzle images and visualize model performance with metrics and confusion matrices.
Main Code File
ARCNN.ipynb: This Jupyter notebook contains all the code for data preprocessing, model training, evaluation, and prediction. It is structured as follows:
Data Preprocessing: Loading, cleaning, and preprocessing the dataset. This includes resizing and normalizing the images, as well as splitting them into training and test sets.
Model Definition (ARCNN): Defines the ARCNN model architecture, which is a Convolutional Neural Network (CNN) with attention and residual blocks for better feature extraction and classification performance.
Model Training: Trains the ARCNN model on the preprocessed images, adjusting hyperparameters and fitting the model to the training data.
Model Evaluation: Evaluates the trained model on the test set and computes key metrics such as accuracy, precision, recall, and F1 score.
Prediction: Uses the trained model to predict whether extrusion occurred or not on new images of the 3D printer nozzle.
Visualization: Includes visualizations like accuracy/loss curves, confusion matrices, and feature maps.
Instructions for Running the Code
1. Clone the Repository
bash
Copy code
git clone https://github.com/MysticalDawn/3D-Printer-Error-Detection-Final.git
cd 3D-Printer-Error-Detection-Final
2. Install Dependencies
Create a virtual environment (recommended) and install the required libraries using:

bash
Copy code
pip install -r requirements.txt
3. Open the Notebook
Launch Jupyter Notebook and open the ARCNN.ipynb file:

bash
Copy code
jupyter notebook
Then, open the ARCNN.ipynb file from the Jupyter interface.

4. Run the Cells
The notebook is organized into cells. Run each cell sequentially:

Data Preprocessing: The notebook will load and preprocess the image dataset (resizing, normalization, and data splitting).
Model Definition and Training: The ARCNN model will be defined and trained on the preprocessed images.
Model Evaluation: After training, the model's performance will be evaluated, and metrics such as accuracy, precision, recall, and F1 score will be displayed.
Prediction and Visualization: The notebook will make predictions on new nozzle images and display results such as confusion matrices and model performance visualizations.
5. Make Predictions
After training, use the notebook to predict whether extrusion occurred or not in new 3D printer nozzle images. The notebook will output predictions for the input images.

Dataset
The dataset used in this project contains images of 3D printer nozzles. These images are labeled to indicate whether extrusion occurred or not. You can download the dataset from the Kaggle competition here.

Results
The ARCNN model can accurately classify nozzle images based on whether extrusion occurred. The model’s performance is evaluated using various metrics, and results are shown in the evaluation section of the notebook.

License
This project is licensed under the MIT License - see the LICENSE file for details.

Acknowledgements
Kaggle for providing the dataset.
TensorFlow/Keras for implementing and training the ARCNN model.
scikit-learn for machine learning evaluation.
The original authors of ARCNN for model architecture inspiration.
