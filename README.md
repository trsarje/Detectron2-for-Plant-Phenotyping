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


## Results

![Sample Image](https://github.com/trsarje/Detectron2-for-Plant-Phenotyping/blob/master/result/Result.png "1")
