# Project 'Object Classification and Detection'

---

![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
![Azure](https://img.shields.io/badge/azure-%230072C6.svg?style=for-the-badge&logo=microsoftazure&logoColor=white)

This project was made for the **'Artificial Intelligence'** course in my university.

I used **Azure's Computer Vision** resource to classify the objects found in the images I provided as input 
and then for those that have a bike to detect the position of the bicycle.

One example of a result for the classification part:
- Image with a bike and a person:


    bike07.jpg:
    {'additional_properties': {}, 'rectangle': <azure.cognitiveservices.vision.computervision.models._models_py3.BoundingRect object at 0x12ba5de90>, 'object_property': 'person', 'confidence': 0.8, 'parent': None}
    {'additional_properties': {}, 'rectangle': <azure.cognitiveservices.vision.computervision.models._models_py3.BoundingRect object at 0x12ba5df90>, 'object_property': 'bicycle', 'confidence': 0.859, 'parent': <azure.cognitiveservices.vision.computervision.models._models_py3.ObjectHierarchy object at 0x12ba5e050>}

- Image with just a bike:


    bike09.jpg:
    {'additional_properties': {}, 'rectangle': <azure.cognitiveservices.vision.computervision.models._models_py3.BoundingRect object at 0x12ba5c8d0>, 'object_property': 'bicycle', 'confidence': 0.777, 'parent': <azure.cognitiveservices.vision.computervision.models._models_py3.ObjectHierarchy object at 0x12ba5c990>}

- Image with just a person:


    bike08.jpg:
    {'additional_properties': {}, 'rectangle': <azure.cognitiveservices.vision.computervision.models._models_py3.BoundingRect object at 0x12b697a10>, 'object_property': 'person', 'confidence': 0.918, 'parent': None}

- Images with multiple objects


    bike06.jpg:
    {'additional_properties': {}, 'rectangle': <azure.cognitiveservices.vision.computervision.models._models_py3.BoundingRect object at 0x12ba6e6d0>, 'object_property': 'car', 'confidence': 0.634, 'parent': <azure.cognitiveservices.vision.computervision.models._models_py3.ObjectHierarchy object at 0x12ba6e790>}
    {'additional_properties': {}, 'rectangle': <azure.cognitiveservices.vision.computervision.models._models_py3.BoundingRect object at 0x12ba6e850>, 'object_property': 'person', 'confidence': 0.734, 'parent': None}
    {'additional_properties': {}, 'rectangle': <azure.cognitiveservices.vision.computervision.models._models_py3.BoundingRect object at 0x12ba6e990>, 'object_property': 'person', 'confidence': 0.801, 'parent': None}
    {'additional_properties': {}, 'rectangle': <azure.cognitiveservices.vision.computervision.models._models_py3.BoundingRect object at 0x12ba6ead0>, 'object_property': 'cycle', 'confidence': 0.591, 'parent': <azure.cognitiveservices.vision.computervision.models._models_py3.ObjectHierarchy object at 0x12ba6eb50>}
    
    bike10.jpg:
    {'additional_properties': {}, 'rectangle': <azure.cognitiveservices.vision.computervision.models._models_py3.BoundingRect object at 0x12ba7c210>, 'object_property': 'Gondola', 'confidence': 0.516, 'parent': <azure.cognitiveservices.vision.computervision.models._models_py3.ObjectHierarchy object at 0x12ba7c2d0>}
    {'additional_properties': {}, 'rectangle': <azure.cognitiveservices.vision.computervision.models._models_py3.BoundingRect object at 0x12ba7c350>, 'object_property': 'bicycle', 'confidence': 0.823, 'parent': <azure.cognitiveservices.vision.computervision.models._models_py3.ObjectHierarchy object at 0x12ba7c490>}


### Metrics

For some of the images I tested the resource, in the Jupyter Notebook you can see some metrics like IoU, Precision and Recall.
On the images you can see with blue the real positioning of the bike, with red the one found by the resource 
and with a transparent green you can see the intersection of the two. 