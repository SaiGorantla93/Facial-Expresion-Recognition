# Facial-Expresion-Recognition

Facial expression recognition has been a challenge for many years. With the recent growth in machine learning, a real-time facial expression recognition system using deep learning technology can be useful for an emotion monitoring system for Human-computer interaction (HCI). I proposed a Facial Expression System that monitors the expressions of the face and captures the changed expression in the live video from webcam. I designed a Convolutional Neural Network model and used it to train different facial expression images with the TensorFlow machine learning library. The system recognizes the five universal emotions, angry, disgust, happy, surprise and sad.​

​The main goal is to design a python-based Facial Expression Detection System that can detect the expression of the face present in the live video from webcam and monitor the webcam for change in the expression and return the latest or current expression present on the webcam to allow changing how a system responds to the user. ​

I Used tensorflow and opencv and trained the mobilenet model using custom dataset.
Steps Required for Executing
Please install python.
The first step is installing pip
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
python get-pip.py
Add Pip to Windows Environment Variables
Install tensorflow dependency
pip install tensorflow
Install OpenCV dependency
pip install opencv-python
I’ve downloaded, saved and loaded my cascade classifier in the program.
Now train the network with the following command
python retrain.py --output_graph=retrained_graph.pb --output_labels=retrained_labels.txt --
architecture=MobileNet_1.0_224 --image_dir=images
execute the program with the following command:
python label.py
