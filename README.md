## 1.	Module Name:  Data Preparation
* Step 1: START
* Step 2: Collect data i.e. collect different hairstyle photos of different face shape
* Step 3: Prepare the database of different face shape like: heat, long, oval, round, square etc. 
* Step 4: Sorting of collected data i.e. organize or sort the collected data into respective databases according to face shape 
* Step 5: END

## 2.	Module Name:  Face Detection
* Step 1: START
* Step 2: Importing required libraries for e.g. import cv2
* Step 3: Load the cascade with the function cascadeClassifier for importing harcascade_frontalface_default.xml file.
* Step 4: Input the image from user for recommending hair style 
* Step 5: Converting user’s image into grey scale image
* Step 6: Detecting face in the image by the function detectMultiScale().
* Step 7: Draw rectangle around faces to show the result of face detection module
* Step 8: END

## 3.	Module Name:  Face Landmark Detection
* Step 1: START
* Step 2: Import the required libraries for e.g. numpy , dlib 
* Step 3: import shape_predictor_68_face_landmarks.dat file into respected directory
* Step 4: Input the user’s image 
* Step 5 : Convert the image into grey scale image
* Step 6: Detect the face using detector() function
* Step 7: Detect the landmarks using predictor() function
* Step 8: Display the landmarks by drawing the circles around the key / landmark points 
* Step 9: END

## 4.	Module Name:  Face Shape Detection
* Step 1: START
* Step 2: Import required libraries like: beautifulSoup , pandas , pathlib , kmeans etc
* Step 3: Apply kmeans on image who’s landmark is detected to differentiate between hair and skin
* Step 4: Apply following steps to get length of forehead
* 1. get midpoint of forehead
*	2. travel to right and left side
* 3. detect the corners of forehead which is nothing but hairs
* Step 5: drawing lines on forehead with circles
* Step 6: Calculating angle between the landmarks that we calculated by using arcustangens.
* Step 7: Calculating similarity between the landmarks 
* Step 8: Face shape is detected by considering the conditions
* Step 9: Display output
* Step 10: END

## 5.	Module Name:  Recommend Best Suited Hairstyle
* Step 1: START
* Step 2: Input the hair length either long or short, input the hairstyle should be updos or not
* Step 3: Input the image from user
* Step 4: Processing of image. Processing includes noise removal, face detection, face landmark detection, and face shape detection
* Step 5: Recommending the appropriate hairstyle. Here the detected face shape is used to fetch the images from databases
* Step 6: display the recommended images along with their percentage of best suited on user’s face.
* Step 7: END
