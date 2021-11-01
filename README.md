# Tensorflow Demo
This repository contains an introduction in machine learning using Tensorflow.
Sample programs are provided as Jupyter Notebooks. Presentation slides can be
found [here](https://github.com/rzbrk/ml-demo/raw/dietpi/ml-demo.pdf)

## Launch Jupyter Notebooks
This requires that the Python virtual environment is already set up. If not,
follow the installation instructions below.

From within the repository directory execute:
```
pipenv run jupyter notebook
```

## Installation
This manual describes the installation of Tensorflow on a Raspberry Pi
microcomputer running the OS [Raspberry Pi OS](https://www.raspberrypi.com/software/).

Tested with:
* Raspberry Pi 4, 8 GB RAM (4 GB of RAM should be sufficient)
* Raspberry Pi OS 2021-05-07 (based on Debian Buster)

The above Raspberry Pi OS version features Python 3.7.

### Clone repository and select correct branch
```
git clone https://github.com/rzbrk/ml-demo.git
cd ml-demo/
git checkout raspios
```

### Install dependencies
```
sudo ./dependencies.sh
```

### Download tensorflow wheel for Raspberry Pi architecture (aarch64)
```
./tensorflow-2.5.0-cp37-none-linux_armv7l_numpy1200_download.sh
```
This will download the wheel file in the current directory.

### Establish virtual Python environment using pipenv
On the Raspberry Pi this step can take quite a while!
```
pipenv install # Install from Pipfile
pipenv install tensorflow-2.5.0-cp37-none-linux_armv7l.whl
```

### Aknowledgements
The Jupyter Notebooks are based on https://github.com/lmoroney/mlday-tokyo and
the tutorials on the [Tensorflow
website](https://www.tensorflow.org/tutorials/keras/classification).
The installation manual is based on https://github.com/PINTO0309/Tensorflow-bin.

