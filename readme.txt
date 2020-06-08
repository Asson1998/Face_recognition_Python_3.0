This is a fully functional Face recognition module . To start with , download all the required libraries :-

# install Dlib Toolkit
pip install dlib

# Install Face_recognition module
pip install face_recognition

# install imutil package
pip install imutils

# considering you have downloaded all the obvious libraries and modules like python and opencv etc.

___________________________________________________________________

# Make directory in Dataset folder & name it whose face to put in it. (currently name Name-1 , Name-2 etc with no pictures)
# Put 3 to 6 photos of the person
# and run  the following command in terminal to train the added faces.

python encode_faces.py --dataset dataset --encodings encodings.pickle \
	--detection-method hog


#Then run the following command to activate face recognition

python pi_face_recognition.py --cascade haarcascade_frontalface_default.xml \
	--encodings encodings.pickle



____________________________________________________________________

There is a file 01_face_dataset.py which is used to click 6 photos.
____________________________________________________________________