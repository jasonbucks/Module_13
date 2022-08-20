# Module_13 - Neural Networks

   ![Charts Picture](Images/13-4-challenge-image.png)

As a risk management associate at Alphabet Soup, a venture capital firm, I am tasked with creating a model that predicts whether startup applicants for funding will be successful or not.  Using a CSV file containing over 34,000 organizations that have received funding from Alphabet Soup over the years, as well as my knowledge of machine learning and neural networks, I will use the features included in this dataset to create a binary classifier model that predicts whether or not a startup becomes a successful business.

---

## Technologies

This Jupyter Notebook was uploaded and run in Google Colab to help with issues with FB Prophet running on my machine via Jupyter Labs.  To access the notebook directly from my Google Colab Drive, navigate to https://colab.research.google.com/drive/1TLFneEL1z_A8PuZFJL9osUKnEK5Cv7LN?usp=sharing 

It leverages python 3.7.11 with the following packages:

* [pandas](https://pandas.pydata.org) - Use the Pandas library, along with JupyterLab, to collect, prepare and analyze data.

* [scikit-learn](https://github.com/scikit-learn/scikit-learn) - a Python module for machine learning built on top of SciPy.

* [tensorflow](https://www.tensorflow.org/) - TensorFlow makes it easy for beginners and experts to create machine learning models.

---

## Installation Guide

Before running the application first import the following libraries and dependencies:

```python
  import pandas as pd
  from pathlib import Path
  import tensorflow as tf
  from tensorflow.keras.layers import Dense
  from tensorflow.keras.models import Sequential
  from sklearn.model_selection import train_test_split
  from sklearn.preprocessing import StandardScaler,OneHotEncoder
```

---

## Usage and Analysis

The notebook has 3 main subsections, each of which contain the instructions as well as my code.
* Step 1: Prepare the data for use on a neural network model
* Step 2: Compile and evaluate a binary classification model using a neural network
* Step 3: Optimize the neural network model using several different methods

To optimize the neural network model, I tried several different methods.  First was to reduce the size of the dataset by eliminating features that were very rarely used.  Other optimization methods were to add extra hidden layers as well as adding extra nodes in these hidden layers.  Despite all of these attempts, the accuracy rate for all of my neural network models hovered right around 0.730 for all alternatives, and the loss rate was also relatively stable at around 0.555.  While this doesn't necessarily mean that there is no way to further optimize my original model, it does say that my original model is a pretty good starting point for future analysis.

---

## Contributors

Starter code was provided by UW Fintech Bootcamp.  Updates and analysis by Jason Buckholt.  

---

## License

MIT License

Copyright (c) 2022 Jason Buckholt

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
