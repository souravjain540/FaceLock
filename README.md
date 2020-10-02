PROBLEM STATEMENT
The security of applications in mobile phones or website’s is always a major issue to ensure the security and privacy design a Machine Learning Algorithm which will only unlock the application or website when it will scan your face.

OBJECTIVE AND SCOPE
The objective of the project is to provide user an algorithm which will detects the face of the user and unlock the applications or website’s according to that.
It will first take the training data as an input from the camera of the device and then will train the model from the input and will detect the face according to that training of the model.

METHODOLOGY
There will be two modules in this project namely “Mod1” and “Mod2”.
Mod1 :-
In the first module by the use of OpenCV library of Python :-

1. We will define the “Haarcascade_frontal_face” classifier as the face classifier to detect only the front face of the user for the face lock not background or any other feature.

2. We will initialize webcam using “ cv2.VideoCapture(0)”.

3. We will start capturing images by converting it into “black and white color” and we will crop the image too

4. If face is detected according to face classifier then it will capture the image otherwise “Face Not Found” will be shown .

5. This process will go until 1000 pics are captured or enter key is pressed.

6. Store Pics to given path.
                                                      

Mod2:-
1. Define the path where pics are and then read and load pics using cv2.imread() method.

2. Define the model which we have selected as “ cv2.face.LBPHFaceRecognizer_create()”.

3. Train the training data on this model using model.train().

4. Initialize webcam again and again do same cropping and converting of image into black and white.

5. Use “Haarcascade_frontal_face” classifier to detect and capture the face.

6. Use the captured image to predict whether the face matched with the training data or not.

7. If confidence is above 85% then “UNLOCK” otherwise “LOCKED”.

8. “Enter“ Key is used to exit.
                                   

SOFTWARE USED

Python :-  We have used python latest version “ 3.8.5” in the project.

OpenCV :- OpenCV (OPEN SOUCE COMPUTER VISION) is an open-source BSD-licensed library that includes several hundreds of computer vision algorithms. We will use many methods of opencv in this project.

Anaconda :- Anaconda Enterprise is an enterprise-ready, secure, and scalable data science platform that empowers teams to govern data science assets, collaborate, and deploy data science projects.

HARDWARE USED
A windows system with webcam in it.

