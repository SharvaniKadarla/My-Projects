
# OBJECT RECOGNITION USING R

The objective of this case study is to demonstrate Image classification and detection of objects using R language. 


## Introduction
A computer vision technology called Object Recognition can be used to locate items in photos or movies. Object recognition is the area of artificial intelligence (AI) concerned with the abilities of robots and other AI implementations to recognize various things and entities. It allows robots and AI programs to pick out and identify objects from inputs like video and still camera images. Object recognition is a key output of deep learning and machine learning algorithms. Humans are adept at identifying individuals, objects, settings, and other visual elements when viewing photographs or videos. 

The objective is to train a computer to perform something that comes effortlessly to people: grasp what an image conveys. Driverless automobiles use object recognition as a fundamental technology to identify a stop sign or tell a pedestrian from a lamppost. It is also helpful in many different applications, including robotic vision, industrial inspection, and illness identification in bioimaging. Various methods can be used for object recognition. Deep learning and machine learning methods have recently gained popularity as solutions to object recognition issues. Both methods teach users how to recognise items in pictures, but they operate in different ways. The main purpose of object detection is to identify and locate one or more effective targets from still image or video data. 

## Explanation about the topic
Object recognition  refers to a collection of related tasks for identifying objects in digital photographs.

- Region-Based Convolutional Neural Networks, or R-CNNs, are a family of techniques for addressing object localization and recognition tasks, designed for model performance.

- Image classification: Algorithms produce a list of object categories present in the image.

- Single-object localization: Algorithms produce a list of object categories present in the image, along with an axis-aligned bounding box indicating the position and scale of one instance of each object category.


**Object detection**: Algorithms produce a list of object categories present in the image along with an axis-aligned bounding box indicating the position and scale of every instance of each object category.

The performance of a model for image classification is evaluated using the mean classification error across the predicted class labels. The performance of a model for single-object localization is evaluated using the distance between the expected and predicted bounding box for the expected class. Whereas the performance of a model for object recognition is evaluated using the precision and recall across each of the best matching bounding boxes for the known objects in the image.

**Object recognition** is a computer vision technique for identifying objects in images or videos. Object recognition is a key output of deep learning and machine learning algorithms. When humans look at a photograph or watch a video, we can readily spot people, objects, scenes, and visual details. The goal is to teach a computer to do what comes naturally to humans: to gain a level of understanding of what an image contains.

Object recognition is a key technology behind driverless cars, enabling them to recognize a stop sign or to distinguish a pedestrian from a lamppost. It is also useful in a variety of applications such as disease identification in bioimaging, industrial inspection, and robotic vision.

![Object Recognition Flow Chart](https://i.postimg.cc/d3PxJVPm/1.png)


## Code Explanation
**Classify** : Here image_darknet_model is the function from the image.darknet package and there are 4 arguments in it, called as below and assigning the result to the variable named “darknet_model”

- type : This can be set to either classify or detect
- model : We’re going to use a pre-trained model from image.darknet package. For classification, we’ll use a model called “tiny.cfg”
- weights : The weights for this model are stored in a file on your computer, in the same location as where this package was installed or if it the package was by default or in-built in online compilers. The weights we’re interested in for classification for this particular model is called “tiny.weights”.
- labels : This also is going to be stored in a file on your computer, in the same location as where this package was installed or if it the package was by default or in-built in online compilers. And for this model, the labels are stored in “imagenet.shortnames.list”

Here, we’re going to actually apply this model onto an image. To do that we’re going to use image_darknet_classify function of 2 arguments specified as
- file :  Copy and paste the path of the image file which needs to classified
- object : Pass the model which we created in the previous step

**Detect** : Here image_darknet_model is the function from the image.darknet package and there are 4 arguments in it, called as below and assigning the result to the variable named “darknet_model”

- type : This can be set to either classify or detect
- model : We’re going to use a pre-trained model from image.darknet package. For detection, we’ll use a model called “tiny-yolo-voc.cfg”
- weights : The weights for this model are stored in a file on your computer, in the same location as where this package was installed or if it the package was by default or in-built in online compilers. The weights we’re interested in for classification for this particular model is called “tiny-yolo-voc.weights”.
- labels : This also is going to be stored in a file on your computer, in the same location as where this package was installed or if it the package was by default or in-built in online compilers. And for this model, the labels are stored in “voc.names”

**System.file()**:Finds the full file names of files in packages etc.

          system.file(…, package = "base", lib.loc = NULL, mustWork = FALSE)

      Arguments:
      character vectors, specifying subdirectory and file(s) within some package.
      default, none, returns the root of the package. Wildcards are not supported.

- package: a character string with the name of a single package. An error occurs if more than one package name is given.
- lib.loc: a character vector with path names of R libraries. 
- mustWork: logical. If TRUE, an error is given if there are no matching files.

We’re using image_darknet_detect function with 2 arguments passed into it

- file :  Copy and paste the path of the image file which needs to detected
- object : Pass the model which we created in the previous step
Now run the code to see the output.

After executing all the code cells, then we can observe the new file named “predictions.png”  in the left side of the files panel where we have uploaded the image for getting predictions, and hence this is the output.

## Output Screens
![House](https://i.postimg.cc/5NqL7NPd/house.png)

![HousePred](https://i.postimg.cc/RZ5pfFNk/house-pred.jpg)


![TV](https://i.postimg.cc/6Qs7tkbL/TV.jpg)

![TV PRED](https://i.postimg.cc/2yJkTWPF/TV-PRED.jpg)


![Cycle](https://i.postimg.cc/R09Hcr1C/cycle.jpg)

![Cycle Pred](https://i.postimg.cc/mg79zZH6/cycle-pred.png)


![Road](https://i.postimg.cc/fR3NBkKB/road.jpg)

![Road Pred](https://i.postimg.cc/3xGqkG95/road-pred.jpg)


![Cat Dog](https://i.postimg.cc/NfCyK9F4/cat.jpg)

![Cat Dog Pred](https://i.postimg.cc/Tw2Gj0HW/catpred.jpg)
