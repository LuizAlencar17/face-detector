# Python project to detect faces

![Example](https://github.com/LuizAlencar17/face-detector/blob/main/GIFs/example.gif?raw=true)

Face recognition project developed in Python. The project is divided into three stages: 1) image capture and treatment; 2) training and evaluation of an artificial intelligence model; and 3) capture and classification of images by the webcam

## Installation

You need to install some libraries.

```bash
pip install tensorflow
pip install keras
pip install matplotlib
pip install Pillow
pip install tensorflow 
pip install shutil 
pip install mtcnn 
pip install numpy
```

## Files

The repository is organized as follows:

#### 1. Dataset


```bash
/dataset
-------- /faces
-------- /photos
```

#### 2. Face detector
This folder contains the files for the face detector model.

```bash
/face_detector
-------- /deploy.prototxt
-------- /res10_300x300_ssd_iter_140000.caffemodel
```

#### 3. File to capture photos
In this file you can create your dataset, capturing photos and extracting only people's faces. In each captured photo, 3 face photos are extracted, because after the face is extracted from a photo, it is rotated in two directions, generating two new images automatically.

```bash
step1_extract-faces-from-webcam.ipynb
```

#### 4. Model training
In this file you can train and evaluate your artificial intelligence model. The model that is used in this project is a neural network called MobileNetV2.

```bash
step2_train-and-evaluation_face-recognize.ipynb
```

#### 5. Using the model on the webcam
After the capture and training process is done, you can run this file to perform real-time face classification by your webcam

```bash
step3_webcam_face-recognize.ipynb
```

   ## License

This project is licensed under the MIT License - see the [LICENSE](https://opensource.org/licenses/MIT) page for details.