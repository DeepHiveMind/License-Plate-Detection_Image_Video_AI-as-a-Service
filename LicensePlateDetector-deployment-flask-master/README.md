# Text-Language-Detection-in-Image
Detects and Recognizes text and font language in an image
## Description
Performed this analysis using The Tesseract OCR Engine.


The Project consist of following steps : 

1.) The first step is a connected component analysis in which outlines of the components are stored into Blobs<br />
2.) Blobs are organized into text lines and broken into words<br />
3.) Recognize every word in a two-pass process<br />
4.) A final phase resolves fuzzy spaces, and finalize text<br />


## Prerequisites

# Software
* libtesseract (>=3.04)
* libleptonica (>=1.71)
* Cython
* Pillow
* tesserocr
* Python 2.7.0 |Anaconda 4.3.0 (64-bit)|<br />

Tested on Ubuntu 16.04 LTS amd64 xenial image built on 2017-09-19 8-core CPU


## Installation

```
sudo apt-get update -y
sudo apt-get upgrade -y
sudo apt-get install python-dev python-pip
sudo apt-get install tesseract-ocr-all libtesseract-dev libleptonica-dev
pip install Cython
pip install Pillow
pip install tesserocr
```


## Running

* Simply Clone the repository and run this command from root directory.

```
python ocr_itt.py -i <image_path.jpg>

```

       
## Input 1
```$ python ocr_itt.py -i e.jpg``` <br/>
![e](https://user-images.githubusercontent.com/15799933/31809000-60ffe726-b593-11e7-95ab-e29f7c6d8153.jpg)

## Output
```
English
Confidence score is 78.6614583333
```
## Input 2
```$ python ocr_itt.py -i h.jpg``` <br/>
![h](https://user-images.githubusercontent.com/15799933/31809002-619ba3aa-b593-11e7-800f-8147d357b6e0.jpg)

## Output
```
Hindi
Confidence score is 84.2118644068
```
## Input 3
```$ python ocr_itt.py -i s.jpg``` <br/>
![s](https://user-images.githubusercontent.com/15799933/31809001-614bb534-b593-11e7-8c40-6cc07e5c6738.jpg)

## Output
```
Spanish
Confidence score is 69.7443609023
```

# LicensePlateDetector-deployment-flask
Deployment of ML model using flask

Flask is a web application framework written in Python. I have deployed my previous project of LicensePlateDetector using Flask as an api.
This is an easy and quick way to see your models in production.

#### Setup

1. Clone the repository
2. Run api.py. (Make sure Apache server is running)
3. Go to localhost:8000 to see your application in action. (Port 8000 has been configured in api.py)

 ![img1](https://user-images.githubusercontent.com/19779081/50811360-f9fedc80-1333-11e9-91e2-32e2110df052.PNG)
 
4. Browse an input image of car ( can download from my LicensePlateDetector repo). Click on Detect License Plate

![img2](https://user-images.githubusercontent.com/19779081/50811428-3c281e00-1334-11e9-91ea-1a4a18b6fff8.PNG)

5. Click on segment characters to segment the license plate.

![img3](https://user-images.githubusercontent.com/19779081/50811462-64178180-1334-11e9-84c8-8cbafed9349c.PNG)

6. On clicking of Predict Characters, ML trained model is loaded and is used for prediction of characters of plate.

![img4](https://user-images.githubusercontent.com/19779081/50811485-92955c80-1334-11e9-9ef9-1829d701b6f1.PNG)

A brief description about the process is mentioned in the description tab.

![img5](https://user-images.githubusercontent.com/19779081/50811547-dc7e4280-1334-11e9-8419-8e045d8d0c90.PNG)

