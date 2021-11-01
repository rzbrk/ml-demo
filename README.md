# Tensorflow Demo
This repository contains an introduction in machine learning using Tensorflow.
Sample programs are provided as Jupyter Notebooks. Presentation slides can be
found [here](https://github.com/rzbrk/ml-demo/raw/x86-64/ml-demo.pdf)

## Launch Jupyter Notebooks
This requires that the Python virtual environment is already set up. If not,
follow the installation instructions below.

From within the repository directory execute:
```
pipenv run jupyter notebook
```

## Installation
This manual describes the installation of Tensorflow on a x86-64 microcomputer
running a typical Linux OS.

Tested with:
* Lenovo Thinkpad T460  
* Arch Linux (kernel 5.14.14 as of 2021/10/20)

Arch Linux at the time of writing features Python 3.9.

### Clone repository and select correct branch
```
git clone https://github.com/rzbrk/ml-demo.git
cd ml-demo/
git checkout x86-64
```

### Establish virtual Python environment using pipenv
```
pipenv install # Install from Pipfile
```

### Aknowledgements
The Jupyter Notebooks are based on https://github.com/lmoroney/mlday-tokyo and
the tutorials on the [Tensorflow
website](https://www.tensorflow.org/tutorials/keras/classification).
The installation manual is based on https://github.com/PINTO0309/Tensorflow-bin.

