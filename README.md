# Face-Mask-Alert-System---RTAP
Face Mask Alert System using Convolutional Neural Network and alert message is sent through Simple Mail Transfer Protocol (SMTP).
<br>
## Dependencies
**1. smtplib**<br>
**2. opencv**<br>
**3. matplotlib**<br>
**4. Tensorflow**<br>
**5. Keras**<br>

## Working
The dataset for this face mask alert system has been taken from the [github repository](https://github.com/prajnasb/observations/tree/master/experiements/data).The dataset consists of two folders namely with mask and without mask. The data in two folders are equally distributed in the form of RGB images.<br>
The images in the dataset are then converted into gray scale image and then normalised in the range of 0 to 1. The Convolutional neural network in the tensorflow framework deals with numerical value , thus the image list containing images are converted into numpy array and the two target "with mask , without mask" are also converted into categorical values and stored in a numpy array.<br>
The data in the dataset are then split into training and test data and CNN technique is performed . The generalised model is then saved using Checkpoint function from keras.callbacks library and the saved model is then used for detecting mask.<br>
The cascadeClassifier xml file is used to detect the frontal face of a person and the model run on that algorithm and the face mask detection is performed.The face with no mask is shown as a warning message(to wear the face mask) and the alert mail is sent to the management server using SMTP technique.<br>

## CNN Architecture





