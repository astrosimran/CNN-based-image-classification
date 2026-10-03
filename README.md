# CNN-Based Image Classification with PyTorch

A deep learning project implementing a **Convolutional Neural Network (CNN)** using PyTorch for image classification on the **MNIST** and **Fashion-MNIST** datasets.
The project also investigates **filter count as a CNN hyperparameter** by comparing models with different numbers of convolutional filters.

## Project Overview
The objective of this project is to:
* Build a CNN using **PyTorch**
* Classify handwritten digits from the **MNIST** dataset
* Experiment with **filter count as a hyperparameter**
* Compare model performance for different filter configurations
* Apply the selected CNN configuration to the **Fashion-MNIST** dataset
* Compare classification performance across the two datasets

## Libraries Used
* Python
* PyTorch
* Torchvision
* NumPy
* Pandas
* Matplotlib
* Google Colab

## 📊 Datasets

### MNIST
MNIST contains grayscale images of handwritten digits from **0–9**.
* 60,000 training images
* 10,000 test images
* Image size: 28 × 28 pixels
* Number of classes: 10

### Fashion-MNIST
Fashion-MNIST contains grayscale images representing **10 clothing categories**.
* 60,000 training images
* 10,000 test images
* Image size: 28 × 28 pixels
* Number of classes: 10

## CNN Architecture
The model consists of:
1. Convolutional Layer
2. ReLU Activation
3. Max Pooling
4. Convolutional Layer
5. ReLU Activation
6. Max Pooling
7. Fully Connected Layer
8. Output Layer
The number of filters in the convolutional layers is treated as a **hyperparameter**.

### Filter Configurations Tested

The following filter counts were compared:
- 8 filters
- 16 filters
- 32 filters
The model performance was evaluated using test accuracy for each configuration.

## Training Configuration

| Parameter                | Value              |
| ------------------------ | ------------------ |
| Optimizer                | Adam               |
| Learning Rate            | 0.001              |
| Loss Function            | Cross Entropy Loss |
| Batch Size               | 64                 |
| MNIST Training Epochs    | 5                  |
| Filter Experiment Epochs | 3                  |
| Fashion-MNIST Epochs     | 5                  |
| Filter Counts            | 8, 16, 32          |

## Hyperparameter Experiment
Filter count controls the number of feature maps produced by the convolutional layers.
The project compares CNN models using: **8 → 16 → 32 filters**
The final test accuracy for each configuration is recorded and compared to identify the configuration that performed best in the experiment.

## Results
The notebook includes:
* Training accuracy vs. epoch
* Test accuracy vs. epoch
* Accuracy vs. number of filters
* MNIST classification results
* Fashion-MNIST classification results

Add your final results here after running the notebook:

| Dataset       | Best Filter Count | Test Accuracy |
| ------------- | ----------------: | ------------: |
| MNIST         |               32  |       99.00 % |
| Fashion-MNIST |               32  |       91.39% |

## Project Structure
CNN-based-image-classification/
│
├── CNN-based-image-classification.ipynb
├── README.md
└── .gitignore
```

## How to Run:

### Option 1 — Google Colab

Open the `.ipynb` notebook in Google Colab and run the cells sequentially.
The datasets are automatically downloaded using `torchvision`.

### Option 2 — Local Environment

Install the required libraries:
bash
pip install torch torchvision numpy pandas matplotlib
Then open the notebook using Jupyter Notebook or JupyterLab.

## Key Learning Outcomes

Through this project, I practiced:
* Building CNN architectures using PyTorch
* Working with image datasets using Torchvision
* Data loading and batching using PyTorch DataLoader
* Training neural networks using backpropagation
* Using Adam optimization and cross-entropy loss
* Evaluating classification accuracy
* Hyperparameter experimentation
* Comparing model configurations
* Applying a trained architecture to different image-classification datasets

## Future Improvements:

Potential improvements include:
* Adding data augmentation
* Using a validation set for hyperparameter selection
* Evaluating the model using a confusion matrix and additional metrics
* Experimenting with learning rate and batch size
* Adding dropout or batch normalization
* Comparing different CNN architectures

## 👩‍💻 Author
**Simran Hotchandani**
Physics Master's Student | IIT Gandhinagar
