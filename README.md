# Object-Detection-with-IensorFlow

# Definition
Object detection is a computer technology related to computer vision and image processing that deals with detecting instances of semantic objects of a certain class (such as humans, buildings, or cars) in digital images and videos. Well-researched domains of object detection include face detection and pedestrian detection. Object detection has applications in many areas of computer vision, including image retrieval and video surveillance. 

# Uses
It is widely used in computer vision tasks such as image annotation, activity recognition, face detection, face recognition, video object co-segmentation. It is also used in tracking objects, for example tracking a ball during a football match, tracking movement of a cricket bat, or tracking a person in a video. 

# Concepts
Every object class has its own special features that helps in classifying the class – for example all circles are round. Object class detection uses these special features. For example, when looking for circles, objects that are at a particular distance from a point (i.e. the center) are sought. Similarly, when looking for squares, objects that are perpendicular at corners and have equal side lengths are needed. A similar approach is used for face identification where eyes, nose, and lips can be found and features like skin color and distance between eyes can be found. 

# Methods
Methods for object detection generally fall into either machine learning-based approaches or deep learning-based approaches. For Machine Learning approaches, it becomes necessary to first define features using one of the methods below, then using a technique such as support vector machine (SVM) to do the classification. On the other hand, deep learning techniques are able to do end-to-end object detection without specifically defining features, and are typically based on convolutional neural networks (CNN).

    Machine learning approaches:
        Viola–Jones object detection framework based on Haar features
        Scale-invariant feature transform (SIFT)
        Histogram of oriented gradients (HOG) features
    Deep learning approaches:
        Region Proposals (R-CNN, Fast R-CNN, Faster R-CNN, cascade R-CNN.)
        Single Shot MultiBox Detector (SSD)
        You Only Look Once (YOLO)
        Single-Shot Refinement Neural Network for Object Detection (RefineDet)
        Retina-Net
        Deformable convolutional networks

# Using Tensorflow Transfer Learning
click the link below to learn more about Tensorflow Transfer Learnling.

https://www.tensorflow.org/lite/models/object_detection/overview

# Setting up the Environment

Now to Download TensorFlow and TensorFlow GPU you can use pip or conda commands:
	
# For CPU
pip install tensorflow
# For GPU
pip install tensorflow-gpu

 

For all the other libraries we can use pip or conda to install them. The code is provided below:
	
pip install --user Cython
pip install --user contextlib2
pip install --user pillow
pip install --user lxml
pip install --user jupyter
pip install --user matplotlib

 

Next, we have Protobuf: Protocol Buffers (Protobuf)  are Google’s language-neutral, platform-neutral, extensible mechanism for serializing structured data, – think of it like XML, but smaller, faster, and simpler. You need to Download Protobuf version 3.4 or above for this demo and extract it.
Now you need to Clone or Download TensorFlow’s Model from Github. Once downloaded and extracted rename the “models-masters” to just “models“.
Now for simplicity, we are going to keep “models” and “protobuf” under one folder “Tensorflow“.
Next, we need to go inside the Tensorflow folder and then inside research folder and run protobuf from there using this command:
	
"path_of_protobuf's bin"./bin/protoc object_detection/protos/

To check whether this worked or not, you can go to the protos folder inside models>object_detection>protos and there you can see that for every proto file there’s one python file created.
