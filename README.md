# MNIST-Classification-Using-a-Mixture-of-Experts-Notebook-

This repository contains a Python implementation that downloads the MNIST dataset, processes it, and then uses a combination of KMeans clustering with decision trees for the "experts", and then combines them in a Mixture of Experts (MoE) approach.

## Description

The code follows these steps:

1. **Downloading and Extracting MNIST Dataset**: Downloads the dataset from Yann LeCun's website and extracts it for further processing.
2. **Loading and Visualizing the Data**: Utilizes `matplotlib` to visualize sample images from the dataset and their distribution.
3. **Processing with PySpark**: Converts the dataset into a PySpark DataFrame and showcases some basic Spark configurations.
4. **Clustering**: Applies KMeans clustering using PySpark's machine learning library to the MNIST dataset.
5. **Training Decision Tree Experts**: For each cluster (from the KMeans clustering), a decision tree classifier (considered as an "expert") is trained.
6. **Mixture of Experts (MoE) Model with TensorFlow**: Combines predictions from different experts using a gating network. The gating network determines the weight of each expert's prediction for a given input.
7. **Training**: Trains the MoE model using TensorFlow.

## Prerequisites

- Jupyter Notebook (install via Anaconda or pip)
- Python 3.x
- Required Libraries:
  - `requests`
  - `gzip`
  - `numpy`
  - `matplotlib`
  - `pyspark`
  - `tensorflow`

You can install the required libraries using `pip`:
```bash
pip install notebook requests numpy matplotlib pyspark tensorflow
```

## Usage

1. Clone this repository:
```bash
git clone [YOUR_REPOSITORY_LINK]
```

2. Navigate to the directory:
```bash
cd [YOUR_DIRECTORY_NAME]
```

3. Start Jupyter Notebook:
```bash
jupyter notebook
```

4. In the Jupyter interface opened in your browser, click on the notebook to open it (`[YOUR_NOTEBOOK_NAME].ipynb`).

5. Run the cells sequentially to execute the code and view the results.


## Results

Once the code is executed, it will:
- Download and extract the MNIST dataset.
- Show a sample of images from the dataset.
- Display Spark configurations.
- Visualize cluster distributions.
- Train Decision Tree models for each cluster.
- Train the Mixture of Experts model.
- (Optional: Display predictions using the MoE model)

Ah, got it! If it's a Jupyter notebook, you might want to provide instructions for setting up and running it within a Jupyter environment. Here's an adjusted README file for your notebook:

## License

This project is licensed under the MIT License.
