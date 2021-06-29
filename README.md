# Vehicle-registration-system

## ABOUT:
The main purpose of this project is to detect a license plate from an image provided by the camera. An efficient algorithm is developed to detect a license plate in various luminance conditions. This algorithm extracts the license plate data from an image and provides it as an input to the stage of Car License Plate Recognition. The image of a vehicle is given as input from the camera and the extracted image of the number plate can be then used for various purposes. This decentralised system can be used to retrieve and check the legitimacy of a number plate and its owner by extracting the complete registration details of the owner. 

#### METHODOLOGY:
Automatic License/Number Plate Recognition (ANPR/ALPR) is a process involving the following steps:
Step #1- Detect and localize a license plate in an input image/frame
Step #2- Extract the characters from the license plate
Step #3- Apply some form of Optical Character Recognition (OCR) to recognize the extracted character
Step #4- Authenticate from database

#### AUTHENTICATION:
Record of an authenticated vehicle along with owner information in residential areas is stored
on the WAMP server. Whenever the vehicle arrives, an ultrasonic sensor detects the distance
and presence of the vehicle. By then the camera will initialize and capture video frames. The
taken image is sent for image processing. By applying image processing algorithms, each
character is segmented in one single image and passed on to a sequential neural network model.
It is intelligent enough to recognize characters from the number plate. The recognized number
is matched with the record database. After that the vehicle status is displayed on the Website
created using the Laravel framework. If the number matches, then no action takes place. If the
number does not match, it means the vehicle is un-authenticate. An email to that effect is sent
through SMTP to the parking management authority.

**Following modules were implemented successfully and outputs have been displayed:**

1. Real Time Vehicle Detection

2. Number Plate Extraction

3. Text Detection

4. Redirection to web application

5. Authentication of Car Details
