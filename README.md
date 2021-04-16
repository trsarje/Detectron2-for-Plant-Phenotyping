# Soyabean Plant Phenotyping Using Detectron2

## Motivation
This project is aimed to monitor the phenotypic traits of a plant to observe the development when the plant is subjected to different environmental conditions. The model is trained to identify different instances of plant Leaf, Stem and Early Leaf. Studying these attributes measures complex traits such as growth, yield and adaption to stress. The traditional phenotyping techniques are demanding in efforts and time to walk across fields and take measurements of length and width of leaves, the height of the plant. The method involved in this project is fast, more accurate and scalable. 

## Data

* The data was collected at Dr. Lobaton's ARoS lab for Soyabean plant. Following are few samples of the images used.  
![Sample Image](https://github.com/trsarje/Detectron2-for-Plant-Phenotyping/blob/master/result/sample.png "1")

* The images were annotated using [VGG annotator](https://www.robots.ox.ac.uk/~vgg/software/via/) in JSON format. 
* The annotations were lables in three categories of "Leaf", "Early_leaf"and "Stem". 
* The JSON annotation were converted in COCO format, suitable for Detectron2 input pipeline. 

![Sample Image](https://github.com/trsarje/Detectron2-for-Plant-Phenotyping/blob/master/result/Annotation.png "1")

## Model
Detectron2 has different frameworks implemented such as Faster RCNN, Mask RCNN, SSD for variour tasks such as object detection, segmantation, keypoint detection. Out of these options, I used Mask RCNN for the instance segmentation. The framework has different back bones available such as VGG, ResNet50, ResNet101. I used ResNet50 for the final model. 

## Results
* The model was trained at different fraction of train data. 
* Final best model results are shown in the following images. 

| No Img to train | Back Bone | Iteration | Box AP@0.5 | Segnemt AP@0.5 |
| --------------- | --------- | --------- | ---------- | -------------- |
| 475             | ResNet 50 | 500       | 42.03      | 39.71          |
| 475             | ResNet 50 | 1000      | 55.61      | 54.52          |
| 380             | ResNet 50 | 500       | 43.86      | 41.26          |
| 380             | ResNet 50 | 1000      | 53.31	     | 51.87          |

![Sample Image](https://github.com/trsarje/Detectron2-for-Plant-Phenotyping/blob/master/result/Result.png "1")
