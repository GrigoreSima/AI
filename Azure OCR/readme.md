# Project 'Azure OCR'

---

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![Azure](https://img.shields.io/badge/azure-%230072C6.svg?style=for-the-badge&logo=microsoftazure&logoColor=white)

This project was made for the **'Artificial Intelligence'** course in my university.

### There are 3 parts in this project:
- **Text recognition on default images**
- **Text detection** (positioning)
- **Text recognition on modified images** (without noise)

## Text recognition on default images
I used **Azure's Computer Vision** resource to recognize text from images with a paper that has written text in Romanian.

![Image with noise](./images/test2.jpeg)

For this image the recognized text by Azure OCR was: 
**Lucces in resolvarea
TEMELOR la
LABORA toarele de
Inteligenta Artificialà!**

### Metrics
- Levenshtein distance
    - CER: 0.08695652173913043
    - WER: 0.6666666666666666
- Jaro distance
    - CER: 0.057971014492753624
    - WER: 0.5555555555555556


## Text detection
I used **Azure's Computer Vision** resource to detect the posioning of each word from the same images.

The result was pretty acurate as you can see in the Jupyter Notebook.


## Text recognition on modified images
I used **Azure's Computer Vision** resource to recognize text from images with a paper that has written text in Romanian **after removing the noise**.

![Image without noise](./images/test2-edited.jpeg)

For this image the recognized text by Azure OCR was: 
**Succes in resolvarea
TEMELOR la
LABORA toarele de
Inteligentà Artificialà!**

### Metrics
- Levenshtein distance
  - CER: 0.08695652173913043
  - WER: 0.6666666666666666
- Jaro distance
  - CER: 0.057971014492753624
  - WER: 0.5555555555555556