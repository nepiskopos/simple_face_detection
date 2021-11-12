# Face Detection


## Description
This repository contains a Jupyter notebook which tests and compares 7 simple face detection Machine Learning algorithms.

The dataset used in these experiments consists of images of families collected from the web. Since most of these images are copyrighted, the dataset is going to remain private.

The face detectors used in these experiments are:
* **OpenCV Haar cascade Face Detector**
* **OpenCV DNN Face Detector**
* **HOG + Linear SVM Face Detector**
* **MMOD + CNN Face Detector**
* **MTCNN**
* **YOLOFace (YOLOv3)**
* **YOLOv5**

The detectors are evaluated based on
* **Total detection time**
* **Total number of faces detected**



## Instructions
### Setup and execution on Ubuntu 20.04

1. Install necessary tools
```console
sudo apt-get -y install wget zip bzip2
```

2. Fetch repository
```console
git clone https://github.com/nbishdev/simple_face_detection.git
```

3. Install Miniconda
```console
wget https://repo.anaconda.com/miniconda/Miniconda3-latest-Linux-x86_64.sh
bash Miniconda3-latest-Linux-x86_64.sh
source ~/.bashrc
```

4. Create a virtual environment for the notebook experiments
```console
conda create -n face
```

5. Install all the necessary packages
```console
conda install -n face -c conda-forge dlib
conda activate face
pip install -r simple_face_detection/requirements.txt
```

6. Execute JupyterLab
```console
jupyter-lab --notebook-dir=simple_face_detection
```
