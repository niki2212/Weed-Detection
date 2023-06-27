# Weed-Detection
Weed Detection using Machine Learning and Image Processing

This project aims to develop a system to detect weeds in pictures using image processing and Support Vector Machine (SVM) algorithm. It involves preprocessing the images, extracting relevant features, and training the SVM model for weed detection.   

The aim is to achieve accurate weed identification and classification. The dataset used for this project is a combination of images having both weeds and plants, the size of the dataset is 2072 images.  This project focuses on weed detection primarily using image processing techniques such as:  
- Conversion to grayscale- To convert the original RGB image to grayscale, so that it can be used for edge detection 
- Adaptive thresholding- This technique automatically determines a threshold value and separate the edges from the background. 
- Morphological opening- To remove noise and small unwanted details. A rectangular kernel of size 3*3 is used for this and it is applied iteratively twice. 
- Dilation- To expand the white regions or foreground in the image to provide a clear distinction from the background. This helps in effective edge detection. 
- Canny edge detection- From the dilated image, we perform canny edge detection on the dilated image obtained above. We highlight the edges as white pixels in the resulting image.  

Store the extracted edge features obtained from the above preprocessing of the images in the form of lists and used them to train support vector machine to learn the edges of both crops and weeds. 80 percent of the images were used for training and 20 percent of the images were used for testing. 

References:  
Muthu, Pabitha. (2021). WEED DETECTION USING IMAGE PROCESSING. 10.13140/RG.2.2.15116.64642. 
