# CoverType Forest Classification with PyTorch

This repository contains a PyTorch-based solution for classifying forest cover types, using a dataset from the UCI Machine Learning Repository. 

The dataset, known as "Covertype," consists of various features related to the characteristics of forests, such as soil type, wilderness area, and various cartographic variables. The target variable is 'Cover_Type,' which describes the type of forest cover.

## Repository Structure

Here is the structure of the project and a brief on files/folders in the repository:

- **covtype.csv**: The Covertype dataset from UCI Machine Learning Repository. This file is not included in the repository but will need to be downloaded and placed in a directory named "Daten Blatt 3."

- **forest_cover_classification.ipynb**: The main Jupyter notebook file that contains the entire project. It consists of data loading, preprocessing, neural network model creation, training, evaluation, and visualization of results.

- **README.md**: The readme file you are currently viewing.

## Model Architecture

The model is a fully connected neural network with six layers. It makes use of batch normalization and the leaky ReLU activation function to handle non-linearities. The Kaiming weight initialization is used to optimize the initial random weights of the neural network.

## Dependencies

To run the project, you will need the following libraries:

- pandas
- torch (PyTorch)
- torchmetrics
- sklearn
- tqdm
- matplotlib
- numpy

You can install these libraries using pip:

```bash
pip install pandas torch torchmetrics sklearn tqdm matplotlib numpy
```

## How to Run

1. Ensure that you have all the required dependencies installed.
2. Download the "Covertype" dataset from the UCI Machine Learning Repository and place it in a folder named "Daten Blatt 3."
3. Open and run the Jupyter notebook (`forest_cover_classification.ipynb`).

## Results

After training the model, the notebook displays a couple of plots showing the training and testing loss, as well as testing accuracy over epochs. The final testing accuracy and loss are printed at the end. These metrics can give you a clear understanding of how well the model is performing.

## Future Work

While the provided model yields a decent performance, there is always room for improvement. You could experiment with different model architectures, try different optimizers, adjust learning rates, or apply various regularization techniques to achieve better results. Additionally, more advanced techniques like cross-validation, hyperparameter tuning, or ensemble learning could be employed for better performance.
