# Face_recognition_system
This repository contains code for facial recognition using openCV and python with a tkinter gui interface on "JETSON NANO BOARD"
If you want to test the code then run train.py file
########################################################################################################################################
Technology used :
-openCV (Opensource Computer Vision)(I m having cv2 version 3.2.0)
-Python(I am using Python 3.6.9)
-tkinter GUI interface(8.6)


Here I am working on Face recognition based Attendance Management System by using OpenCV(Python). One can mark thier attendance by simply facing the camera. 
#########################################################################################################################################
How it works :

When we run train.py a window is opened and ask for Enter Id and Enter Name. After enter name and id then we have to click Take Images button. By clicking Take Images camera of running computer is opened and it start taking image sample of person.This Id and Name is stored in folder StudentDetails and file name is StudentDetails.csv. It takes 60 images as sample and store them in folder TrainingImage.After completion it notify that iamges saved.
After taking image sample we have to click Train Image button.Now it take few seconds to train machine for the images that are taken by clicking Take Image button and creates a Trainner.yml file and store in TrainingImageLabel folder.
Now all initial setups are done. By clicking Track Image button camera of running machine is opened again. If face is recognised by system then Id and Name of person is shown on Image. Press Q(or q) for quit this window.After quitting it attendance of person will be stored in Attendance folder as csv file with name, id, date and time and it is also available in window.

########################################################################################################################################

How to install opencv
 -->   pip3 install opencv-contrib-python


How to install tkinter GUI interface
 --> sudo apt-get install python3-tk

#########################################################################################################################################
Train Recognizer
OpenCV provides three methods of face recognition:
Eigenfaces
Fisherfaces
Local Binary Patterns Histograms (LBPH)
Eigenfaces and Fisherfaces find a mathematical description of the most dominant features of the training set as a whole. LBPH analyzes each face in the training set separately and independently. The LBPH method is somewhat simpler, in the sense that we characterize each image in the dataset locally; and when a new unknown image is provided, we perform the same analysis on it and compare the result to each of the images in the dataset. We will be using the LBPH Face recognizer for our purpose.


For more understanding of LBH Recognizer please  refer " https://towardsdatascience.com/face-recognition-how-lbph-works-90ec258c3d6b "

thanks:
kusum chaudhary
