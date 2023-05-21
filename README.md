# Image-Captioning-Platform-For-Education-Purposes
Generates Arabic captions for images of Laboratory Equipements.


Dataset: [./data/Flickr8k_text/Flickr8k.arabic.full.txt](./data/Flickr8k_text/Flickr8k.arabic.full.txt)

Report: [here](https://drive.google.com/file/d/1vt1LcE_0xEFHpQ95bLWLNWqrwZ9AbTS8/view?usp=sharing)

## Introduction
Image Captioning refers to the art of describing the content of an image by computers. It is a well-known problem in CV and NLP. It has many applications, such as improved information retrieval, early childhood education, for visually impaired persons, for social media, and so on. Although remarkable work has been accomplished recently for English, and due to the lack of large and publicly available dataset, the progress on Arabic Image Captioning is still lagging. Therefore, we developed our own dataset. And this made it a very challanging work to accomplish.

## Model
Inspired by recent advances in neural machine translation, the sequence-to-sequence encoder-decoder approach was adopted here.
![seq2seq-image-captioning-arabic](https://user-images.githubusercontent.com/9033365/50055387-e3ab9980-0156-11e9-859f-dce71314777a.png)

## Results

Results show that developing language specific datasets and end-to-end models outperforms translating English generated captions to a destination language as the later may accumulate both models errors: image captioning and translation.


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


## Citation
Please cite [this paper](https://www.insticc.org/Primoris/Resources/PaperPdf.ashx?idPaper=88812):

```
@conference{visapp20,
author={Obeida ElJundi. and Mohamad Dhaybi. and Kotaiba Mokadam. and Hazem Hajj. and Daniel Asmar.},
title={Resources and End-to-End Neural Network Models for Arabic Image Captioning},
booktitle={Proceedings of the 15th International Joint Conference on Computer Vision, Imaging and Computer Graphics Theory and Applications - Volume 5: VISAPP,},
year={2020},
pages={233-241},
publisher={SciTePress},
organization={INSTICC},
doi={10.5220/0008881202330241},
isbn={978-989-758-402-2},
}
```

## Contact information
For help, issues, or personal communication related to this work, please contact Obeida ElJundi: [oae15@mail.aub.edu](mailto:oae15@mail.aub.edu)
