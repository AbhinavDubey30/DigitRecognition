# DigitRecognition
This project implements a Digit Recognition System using machine learning techniques. The primary goal is to recognize handwritten digits (0-9) from image data, such as the widely used MNIST dataset. The system is trained to accurately predict the digit present in an image by processing pixel values.
Features
**Image Preprocessing:**

Converts raw image data into a format suitable for machine learning models.

**Model Training:**

Uses various machine learning models, such as Logistic Regression, Support Vector Machines (SVM), or Neural Networks, to train the system on digit recognition.

**Accuracy Evaluation:**

Evaluates model performance using accuracy metrics on training and test datasets.
User-Friendly Interface: Includes a basic interface where users can input handwritten digits and receive predictions.

**Project Components**


**Dataset:** Uses the MNIST dataset, which contains 60,000 training images and 10,000 test images of handwritten digits.

**Model Training:** Machine learning algorithms are applied to train models for digit classification.

**Model Evaluation:** The system measures accuracy and performance through confusion matrices, accuracy scores, and loss functions.

**Prediction Interface:** Provides an interface to test the model with custom input images.

# Dependencies
1. `cv2`
2. `sklearn`
3. `skimage`
4. `numpy`
5. `collections`

# Contents
This repository contains the following files-

1. `generateClassifier.py` - Python Script to create the classifier file `digits_cls.pkl`.
2. `performRecognition.py` - Python Script to test the classifier.
3. `digits_cls.pkl` - Classifier file for digit recognition.
4. `photo_1.jpg` - Test image number 1 to test the classifier
5. `photo_2.jpg` - Test image numbre 2 to test the classifier

## Usage 

* Clone the repository - 
```bash
cd 
git clone https://github.com/AbhinavDubey30/DigitRecognition.git
cd digit-recognition
```
* The next step is to train the classifier. To do so run the script `generateClassifier.py`. It will produce the classifier named `digits_cls.pkl`. 

**NOTE** - *I have already created the `digits_cls.pkl`, so this step is not necessary.*
```python
python generateClassifier.py
```
* To test the classifier, run the `performRecognition.py` script.
```python
python performRecognition.py -c <path to classifier file> -i <path to test image>
```
ex -
```python
python performRecognition.py -c digits_cls.pkl -i photo_1.jpg
```

## Results

### Sample Image 1
![Result Number 1](http://hanzratech.in/figures/digit-reco-1-out.png)
### Sample Image 2
![Result Number 2](http://hanzratech.in/figures/digit-reco-2.png)

## TODO

* Add a CNN Based approach
* Reject bounding boxes lesser than some area
* Look into user errors



**Applications**


Handwritten digit recognition in real-time.
Digit identification in scanned documents or forms.
Educational tools for learning machine learning concepts.
