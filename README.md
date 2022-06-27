# Deep Learning Application for Predicting Venture Capital Risk

A binary classification deep neural network model for predicting the success/failure of a venture capital-funded company.


<div class="row">
  <div class="column">
    <img src="./images/vc_cover_image.jpg" alt="Venture Capital Funding" width=95% class='padding'>  
    </div>
</div>


> Builds and optimizes a deep neural network model, trained on over 30,000 companies, to predict a startup's success. 

## Overview of the Analysis

For a venture capital fund to be successful, it is important to evaluate a potential client with as many metrics as possible.  While gathering large amounts of data is essential for proper evaluation, it is too difficult to weigh all the metrics together and translate this into a successful prediction.  Fortunately, a deep neural network model can be trained on metrics taken from companies with known track records, which can then be used to accurately predict the success or failure of a potential startup client of the venture capital fund.  

* The purpose of this application is to build and optimize a deep neural network model for evaluating the potential success of a startup company.  The model will be fit on a scaled dataset of over 30,000 companies with information on their success or failure.

* The features of this model will include:
1) APPLICATION_TYPE
2) AFFILIATION
3) CLASSIFICATION
4) USE_CASE
5) ORGANIZATION
6) STATUS
7) INCOME_AMT
8) SPECIAL_CONSIDERATIONS
9) ASK_AMT


* The prediction to optimize in this model is the binary category:
10) IS_SUCCESSFUL


* For this data set, a IS_SUCCESSFUL value of 0 is a failure, while a value of 1 is a success.

* This analysis will consider three separate binary classification deep neural network models.  The model with the lowest loss, highest accuracy will be considered the most appropriate model to use in predicting the success of a potential startup.  

---
## Technologies

This project is written using a ```Jupyter Lab 3.2.1``` notebook running  ```Python 3.7.11```.  The key libaries are the ```tensorflow 2.9.1```/```keras 2.9.0``` for implementing the deep neural network model.  Additionaly, ```scikit-learn 1.0.2``` is used for implementing the ```StandardScaler``` for scaling the dataset, ```OneHotEncoder``` for separating the categorical data into one-hot numeric arrays, and ```train_test_split``` for separating the data into training and testing subsets.

---

## Installation Guide

Before running the application, first install the following packages if you don't already have them installed in your development environment.

```python
  pip install jupyterlab
```
The scikit-learn libary is automatically installed with the Anaconda installation.  To confirm the install and version number of your scikit-learn libary, run the following command on your command line:
```python
conda list scikit-learn
```
If scikit-learn is not already installed in your environment, run the following in your command line:
```python
pip install -U scikit-learn
```

The TensorFlow 2.0 library should already be installed with the Anaconda installation.  To upgrade and ensure the latest version, run the following command in your terminal:
```python
pip install --upgrade tensorflow
```
To verify a successful installation, run the following after installation:
```python
python -c "import tensorflow as tf;print(tf.__version__)"
```
This should display a TensorFlow version number of 2.0.0 or higher.  If any errors are flagged, visit [TensorFlow Install with pip Guide](https://www.tensorflow.org/install/pip) or [TensorFlow 2 Install Overview](https://www.tensorflow.org/install) for more detailed help.

The Keras package is included with the installation of TensorFlow 2.  To verify the proper install of Keras, run the following command in your terminal:
```python
python -c "import tensorflow as tf;print(tf.keras.__version__)"
```
This should output the latest version number, which should be version 2.2.4 or later.

After a successful installation, ```cd``` into the top folder of the repository.  Then open ```Jupyter Lab``` by typing:
```python
jupyter lab
```
The analysis is performed in the jupyter notebook file named ```venture_funding_with_deep_learning.ipynb```.  

---

## Usage

To view the jupyter notebook used in this analysis, open the ```venture_funding_with_deep_learning.ipynb``` file in a jupyter notebook and run the cells.

The notebook should look like the screenshot below:

<img src="./images/venture_funding_with_deep_learning_screenshot.png" alt="Screenshot of venture_funding_with_deep_learning.ipynb" width="100%"/>

## Data Sources

The venture capital-funded company data used in this report can be found in the Resources directory: ```./Resources/applicants_data.csv```.  The data is provided by the course materials from a UCBerkeley Fintech Extension program.  

---

## Contributors

The seed code is from the course material from a UCBerkeley Extension program.  This analysis is written and performed by John Gruenewald.<br><br>
For more information, contact **John Gruenewald**:<br>
**e-mail:** [john.h.gruenewald@gmail.com](mailto:john.h.gruenewald@gmail.com)<br> **linked-in:**  [jhgruenewald](https://www.linkedin.com/in/jhgruenewald/)<br>**twitter:**  [@GruenewaldJohn](https://twitter.com/GruenewaldJohn)<br>**medium:**  [@comput99](https://medium.com/@comput99)

---

## License

MIT License

Copyright (c) 2022 John Gruenewald