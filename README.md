# Non_helmet_detection_system

Non-Helmet Detection and License Plate Number Extraction

steps:
1.  download and open all ipynb files in jupyter notebook.
2.  Give a video input as video to generate.py (this will convert video to frames).
3.  Pass these frames manually to the person.ipynb(this will show accuracy of both motocycle and person) and choose the image with highest accuracy manually.
4.  Pass this image to helmet.pynb (this will detect whether person is wearing helmet or not by showing accuracy of helmet).
5.  If the accuracy is shown then exit else pass this image to licence_plate_detection_and_extraction.ipynb
6.  licence_plate_detection_and_extraction.ipynb will detect and extract the plate number.




Flow:
1.  In first part the input is given as a video and is converted to frames and these frames are send for detection  
2.	Primarily, detection will happen at three levels using YOLOv3.
3.	In the first level, we will detect the person and the vehicle that they are driving.
4.	In the second level we will detect whether that person is wearing a helmet or not.
5.	In the second level, if the person is not wearing their helmet, then in the last level, we will detect their registration plate and extract their registration plate number using Optical Character Recognition.
6.	Only the objects that are detected will be extracted using Image AI library.
7.	To detect the registration plate, we will have to train our model.
8.	To train our model, we will create a bounding box around the object and extract the numbers into xml and json files.
9.	The above step also involves image pre processing like rotating the image for increased accuracy.
10.	Since this system takes a video input, speed will be of the essence as we need to get our results almost instantaneously, so our aim is to make this a real time detection system.
