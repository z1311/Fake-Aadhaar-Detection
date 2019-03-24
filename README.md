# Fake-Aadhaar-Detection
This project classifies the scanned aadhaar image to either real or fake image by doing two levels of testing. Fake images are the images that are digitally altered. 
## Level 1 Testing
Whenever an image is altered using software tools they leave software signatures in the metadata of the image. Level 1 testing exploit this feature and tries to findout traces of any signature.
It is the fastest and simplest way to classify but there are online tools/websites that helps to clean this type of information in metadata.
MS Paint is a good example that doesn't attach its signature in the metadata of the image.
## Level 2 Testing
It starts of by doing [ELA (Error Level Analysis)](http://fotoforensics.com/tutorial-ela.php) on the image and the result is given to [LBPH (Local Binary Patterns Histograms)](https://towardsdatascience.com/face-recognition-how-lbph-works-90ec258c3d6b)
recognizer which decides whether it is fake or real image. Even though LBPH algorithm is used for face recognition, it can be used in this project for generating histograms and comparing them.




## Block Diagram
![Untitled Diagram](https://user-images.githubusercontent.com/47830313/54882721-fedb2300-4e82-11e9-8fd9-109b9e1eb2f9.jpg)
## Output Screenshots
For selecting image<br />
![Capture1](https://user-images.githubusercontent.com/47830313/54882847-44e4b680-4e84-11e9-934f-c22223889dc1.JPG)<br />
Fake image output screen<br />
![Capture2](https://user-images.githubusercontent.com/47830313/54882851-4e6e1e80-4e84-11e9-94d7-c09bda9204b7.JPG)
![Capture6](https://user-images.githubusercontent.com/47830313/54883072-4f547f80-4e87-11e9-889d-981c95f6de38.JPG)<br />
Real image output screen<br />
![Capture4](https://user-images.githubusercontent.com/47830313/54882857-6180ee80-4e84-11e9-964e-f5e7e2c6807f.JPG)
![Capture5](https://user-images.githubusercontent.com/47830313/54882864-69409300-4e84-11e9-8937-a527b9544341.JPG)
## Tools Used
1. Python 2.7.14
2. OpenCV2
3. Tkinter
4. Pillow
5. Numpy
