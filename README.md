# Face-recognition
  - Using LBPH (Logical binary Pattern Histogram)Algorithm
    -  It basically compares the input facial image with all facial images from a dataset with the aim to find the user that matches that face. It is basically a 1xN comparison
   
#### So Quick question for the one who are absolute bigners
   - from where did i got the LBPH algorithm
   - how to use this Algorithm
   - Is their any other way to do face recognition using other Algorithms
   - what makes this algorithm best from other 2 algorithm which can be used for face recognition
   
     ##### So I have downloaded the opencv package from github which has all the algorithms: https://github.com/opencv/opencv
     so once you download the package navigate to data folder inside it you will find a haarcascade_frontalface_alt.xml file so you can use  that path in your project as i have done in my project check the doc above
     
     #### face_recognizer = cv2.face.LBPHFaceRecognizer_create() 
       - and then you can use face_recognizer to train your model
      ### There are 3 ways according to my knowledge their can be more its on you to search them out and try them all 3 are listed below
        -   EigenFaces – cv2.face.createEigenFaceRecognizer()
        -   FisherFaces – cv2.face.createFisherFaceRecognizer()
        -   Local Binary Patterns Histograms (LBPH) – cv2.face.createLBPHFaceRecognizer()
            - LBPH was my choice because it performs better then other two as internally it works as a histogram and keeps records of all important features realted to a particular person in the from of histogram
### OUTPUT 
![git (2)](https://user-images.githubusercontent.com/42214175/70852682-5fefce80-1eca-11ea-9473-86a3c219e66a.png)
   
### APPLICATIONS
#### This idea can further be developed to make a attendance checking system for any organisatiion its almost very easy to implement and performs good it training and testing data set is provided correctly


### Dataset[Images]
## I have not uploaded the dataset which i have used but you can create your own by making two folders test and train in train folder create subfolders Example mine subfolder had s1,s2,s3,s4 folders in which each folder had images of a particular person 
example folder s3 had all the pictures of Abhishek  and s4 had all the pictures of shubham
 - note all the image should be clear and selfie kind of for each person atleast add 4 to 5 images and they should not be of very high quality otherwise it will get zommed in and will produce error
 #### now coming to test folder it contain single pictures of all the people whose name you want to predict on his/her image
 #### In my case i had 4 people so  there were 4 images in test folder
