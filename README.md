# Face-Recognition

## Background
**IBITF** in collaboration with **Infineon technologies** hosted a hackathon at **IIT Bhilai**, which had a problem statement where the participants were required to classify the given dataset of images on the basis of the faces in the pictures. Above is the code written by our team consisting of [*Abhishek Singh Kushwaha*](https://github.com/ASK-03), [*Siddhi Agarwal*](https://github.com/agaSiddhi) and *Aditya Sharma*.

## Tech Stac
The tech stacks used in the code as mentioned above are →
1. [Face recognition library](https://pypi.org/project/face-recognition/) ( uses dlib library )
2. Pandas
3. Os
4. Numpy 

## Description 
The dataset given consisted of images from the famous TV show FRIENDS. The participants were asked to write a code that one-hot encodes a submission file (.csv file) depending upon whether the character is in the image. 

### Our Approach
Using the face_encodings function of the face recognition library, face encodings of every individual character were extracted by a labelled dataset which consisted of only one image of the respective character (created at the time of the hackathon by our team). The face encodings were compared using the ‘compare_faces’ function, the submission file was created using the list of boolean values returned by the function.

## Installation

To install and use Face-Recognition, follow the steps given below:
- Fork the Face-Recognition repository by clicking the "Fork" button at the top right corner of the repository page. This will create a copy of the repository under your GitHub account.
- Clone the forked repository to your local machine:
  ```
  git clone https://github.com/{YOUR-USERNAME}/Face-Recognition   
  ```
- Navigate to the project directory: 
  ```
  cd Face-Recognition
  ```
- Install the necessary Python packages by running the following command:
  ```
  pip install face-recognition
  ```

## Future Work
The algorithm can be improved to produce much better results, here are some of the approaches that we can use to get better results:
1. Bigger labelled data can be used to get encodings of the character’s face.
    * The mean of encodings can be taken
    * All the encodings can be compared with the encodings present in the test images.
