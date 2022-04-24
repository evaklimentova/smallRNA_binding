# smallRNA_binding

Convolutional Neural Network for prediction of smallRNA:target site binding based on given smallRNA and target sequence.

## Installation

Using Git:
```
git clone https://github.com/evaklimentova/smallRNA_binding.git
```
or
```
git clone git@github.com:evaklimentova/smallRNA_binding.git
```

### Prerequisites

It is implemented in python using Keras and Tensorflow backend.

Required:

* python, recommended version 3.7
    * Keras 2.7.0
    * tensorflow 2.7.0
    * pandas
    * numpy
    
    
### Installing

```
# create a virtual environment:

python -m venv env

# activate it and install the necessary libraries.

source env/bin/activate
pip install -r requirements.txt
```

### Prediction

To make the predictions, choose one of the miRNA (Models/model_miRNA.h5), tRNA (Models/model_tRNA.h5) or yRNA (Models/model_yRNA.h5) models

```
# if you are not actively sourcing from the previously created virtualenv:
source venv/bin/activate
# run the prediction
./predict.py --input <input_file> --output <output_file> --model <Models/model_miRNA.h5>
```

### Web application

The user-friendly web application for miRNA and tRNA target predictions https://evaklimentova.github.io/smallRNA_binding/

