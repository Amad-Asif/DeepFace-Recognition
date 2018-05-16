# DeepFace-Recognition
Tensorflow Implementation of Depp-Face Recognition 

Requirements - 
tensorflow==1.2
scipy
scikit-learn
opencv-python
h5py
matplotlib
Pillow
requests
psutil

Pre Trained Models used  - Inception Resnet V1.0 
Dataset Used - Casia WebFace

Face Aignment using MTCNN Face Detection.

How to - 

Data Perparation

1) Prepare a dataset of images of each person and place them in the Dataset folder in the following format

Deepface Recognition
---Dataset
------Person1
------Person2
.............
.............
.............
------PersonN

2) Create a folder aligned_faces 
3) Run python alignImages.py to crop and align the faces.
4) The file aligned_images/bounding_boxes_28997.txt will cotain the x-axis,y-axis, width, height of the cropped face from the original image. (Not Needed)

Train the classifier

5) Train a classifier, run python trainClassifier.py
6) This will create a classifier at "Deepface Recognition/classifier" directory along with a text file consisting of the key,value pair (ID,Name)

Realtime Recognition - 
