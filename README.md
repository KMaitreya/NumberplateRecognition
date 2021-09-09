# Numberplate Recognition
This is a python project involving computer vision, developed to recognize the text on vehicle numberplates.It has 2 stages:-


a)Numberplate detection-

In this stage the numberplate from the given car image is isolated using opencv functions. The original image is first converted into a grayscale image and then converted into a canny image i.e. an image where the edge are shown. Then the numberplate is detected based on contours and the part of the image containing the numberplate is isolated.

Original image-

![image](https://user-images.githubusercontent.com/47482433/132630541-f8185f18-a825-4123-a926-aaf5ad2699b5.png)

Grayscale image-

![image](https://user-images.githubusercontent.com/47482433/132630577-3003a43a-a3f7-4d72-8480-f6fde6f158a7.png)

Canny image-

![image](https://user-images.githubusercontent.com/47482433/132630608-4072d010-a94a-492e-9926-877b090f5089.png)

Isolated numberplate-

![image](https://user-images.githubusercontent.com/47482433/132630653-c386a873-3675-462e-9892-84ab7893ffe9.png)


b)Optical character recognition-

In this stage the characters on the isolated numberplate image are detected using the easyocr library. The characters are then stored in a variable and then printed.

Result-

![image](https://user-images.githubusercontent.com/47482433/132630908-f28c6450-a625-445e-8223-2504d2551c28.png)

The library used for this function is easyocr(https://github.com/JaidedAI/EasyOCR)

```
pip install easyocr
```

Libraries used-> cv2(opencv), matplotlib, imutils, easyocr
