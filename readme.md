# README

## Environment Setup

### Ensure you have Python 3 installed

### Create a Virtual Environment

Open the command line and run the following command, replacing the path with your project path:

```sh
python -m venv C:\Users\Username\Project\venv
```

### Activate the Virtual Environment

Run the following command:

```sh
C:\Users\Username\Project\venv\Scripts\activate
```

### Install Dependencies

Run the `install_packages.bat` file with the following command:

```sh
C:\Users\Username\Project\install_packages.bat
```

If the virtual environment is already activated, simply run:

```sh
install_packages.bat
```

### Deactivate the Virtual Environment

Once you're done, deactivate the virtual environment by running:

```sh
deactivate
```

### Manually Installing Dependencies

If you prefer not to use `install_packages.bat`, install the required dependencies manually:

```sh
pip install pandas
pip install matplotlib
pip install scikit-learn
pip install tensorflow
pip install torch
pip install torchvision
pip install transformers[torch]
pip install tqdm
pip install transformers
pip install datasets
pip install tf-keras
pip install kagglehub
```

## Running Tasks

### Task 1

Launch Jupyter Notebook and open the file `task1.ipynb`. Execute all the cells sequentially. This notebook automatically creates folders, downloads the MNIST dataset from Kaggle, and processes the data.

**Task Description:**

In this task, you need to use the publicly available MNIST dataset and build three classification models:

1. **Random Forest**
2. **Feed-Forward Neural Network**
3. **Convolutional Neural Network**

Each model should be implemented as a separate class that follows the `MnistClassifierInterface` with two abstract methods—`train` and `predict`. Finally, each model should be managed under a `MnistClassifier` class, which takes an algorithm (`cnn`, `rf`, or `nn`) as input and provides a unified interface for predictions regardless of the selected model.

### Task 2

#### If you need to run Task 2, follow these steps:

1. **`data_make_trans.ipynb`** – Creates a text dataset for transformer training.
2. **`data_make_vision.ipynb`** – Downloads an existing Kaggle dataset with 10 animal classes and splits the data into `train` and `test` sets.
3. **`data_analysis.ipynb`** – Analyzes the datasets used.
4. **`trans.ipynb`** – Fine-tunes a pre-trained model for text classification and saves it in the `trans` folder.
5. **`vision.ipynb`** – Fine-tunes a pre-trained model for image classification and saves it in the `vision` folder.
6. **`task2.ipynb`** – Combines the trained models and executes the main task.

### Task 2 Workflow

1. The user provides a text input, such as *"The image contains a cow."*, along with an image of any of 10 animals. (Butterfly, Cat, Chicken, Cow, Dog, Elephant, Horse, Sheep, Spider, Squirrel)
2. The pipeline determines whether the description matches the image and outputs a boolean value (`True` or `False`).












