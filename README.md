# Image-Captioning-Platform-For-Education-Purposes
Generates Arabic captions for images of Laboratory Equipements.


Dataset: [./data/DataSet_2/Flickr_TextData/Flickr8k.arabic.full.txt](./data/DataSet_2/Flickr_TextData/Flickr8k.arabic.full.txt)

Report: [here]()

## Introduction
Image Captioning refers to the art of describing the content of an image by computers. It is a well-known problem in CV and NLP. It has many applications, such as improved information retrieval, early childhood education, for visually impaired persons, for social media, and so on. Although remarkable work has been accomplished recently for English, and due to the lack of large and publicly available dataset, the progress on Arabic Image Captioning is still lagging. Therefore, we developed our own dataset. And this made it a very challanging work to accomplish.

## Details of The Project:

Project: Image Captioning Platform for Education Purposes

This project aims to develop an image captioning platform for educational purposes, specifically focusing on generating pedagogical descriptions in Arabic from given pictures. The platform will primarily concentrate on laboratory equipment, enabling users to obtain informative descriptions related to the equipment displayed in the images.

The system will consist of two models. The first model will focus on object recognition, leveraging classical machine learning algorithms and tools such as OpenCV, SIFT, and SURF. This model will be trained on a carefully collected dataset of laboratory equipment, enabling it to accurately identify and classify objects within the images.

The second model will be responsible for text generation based on the objects' names provided by the first model. It will employ a sequence-to-sequence (seq2seq) encoder-decoder approach, inspired by recent advances in neural machine translation. This model will be trained to generate coherent and contextually relevant pedagogical descriptions in Arabic, corresponding to the recognized objects.

Once trained and evaluated, the chosen model will be deployed and made accessible through a single-page web application (SPA). This web application will provide a user-friendly interface, allowing users to upload images and receive detailed Arabic descriptions of the laboratory equipment present in the images.

## Key Steps in the Project:

1. Collection of a custom dataset comprising laboratory equipment images.
2. Training of the object recognition model utilizing classical machine learning algorithms and tools like OpenCV, SIFT, and SURF.
3. Evaluation and comparison of different models to select the most effective one.
4. Deployment of the chosen model to a production environment.
5. Development of a SPA web application for convenient model consumption.

## Project's Goal:
The combination of accurate object recognition and the generation of pedagogical descriptions in Arabic will provide a valuable educational resource. This platform will assist students,    educators, and individuals interested in laboratory equipment by offering informative and contextually relevant descriptions in their native language.

## Model:

Inspired by recent advances in neural machine translation, the sequence-to-sequence encoder-decoder approach was adopted here.
![seq2seq-image-captioning-arabic](https://user-images.githubusercontent.com/9033365/50055387-e3ab9980-0156-11e9-859f-dce71314777a.png)


## Installation
1. Clone or download this repository.

2. Make sure python 3.x is installed on your PC. To check if and which version is installed, run the following command:
```
python -V
```
If this results an error, this means that python isn’t installed on your PC! please download and install it from [the original website](https://www.python.org/)

3. (optional) it is recommended that you create a python virtual environment and install the necessary libraries in it to prevent versions collisions:
```
python -m venv myenv
```
where AIC is the environment name. Once you’ve created a virtual environment, you may activate it.
```
myenv\Scripts\activate.bat
```

4. Install required libraries from the provided file (**requirements.txt**):
```
pip install -r requirements.txt
```
Make sure you provide the correct path of **requirements.txt**

5. Open jupyter notebook:
```
myenv\Scripts\jupyter-notebook.exe
```
then navigate to and open [Arabic Image Captioning.ipynb](./Arabic%20Image%20Captioning.ipynb)

## Deployment:

This is our 1st Model "Object recognition" deployment: 
![Res](https://github.com/myyla/Image-Captioning-Platform/assets/96894475/bdb0f9a3-8f01-4cb2-b7c9-d95271d91126)
This is our 2nd Model "Text Generation" deployment:
![WhatsApp Image 2023-05-21 at 15 24 15](https://github.com/myyla/Image-Captioning-Platform/assets/96894475/e2dbef77-4e14-4eb0-be2f-cf69b00194f9)

## Contact information
For help, issues, or personal communication related to this work, please contact us: [amaluth29@gmail.com](mailto:amaluth29@gmail.com) [ibtissam.aoulek@etu.uae.ac.ma](mailto:ibtissam.aoulek@etu.uae.ac.ma) [basma.akarmass@etu.uae.ac.ma](mailto:basma.akarmas@etu.uae.ac.ma)
