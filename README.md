# Counting_objects
Program is designed to detect objects and counting them. 

## Description of the algorithm

1. At the beginning, all the libraries necessary for the operation of the program are imported.
2. Then the image is taken for analysis, the color image is changed to grayscale.
3. Binarization is performed with threshold 120, if the threshold is smaller, interference occurs, if larger, any object disappears from the image and cannot be reproduced.
4. After binarization, counting the area of ​​the objects is performed and calculating how many percent of the image the objects occupy. The number of points on objects and the whole image is displayed.
5. After counting, the operation of opening, i.e. erosion and then dilatation, is performed to disconnect the objects in contact with each other. The structural element used in this operation has dimensions of 3x3, the operation is performed 5 times. At 4 iterations, the objects did not separate, while at 6, smaller objects disappeared. After the opening operation, erosion is performed with iteration = 2. This eliminated errors, i.e. connected objects, but not one hundred percent.
6. Objects in the image are counted and their number and dimensions of the analyzed image are displayed.
7. In the next step, the centers of gravity for the objects are calculated and marked with crosses.
8. In the last step, the Blair-Bliss and Feret ratios are calculated and displayed below.

## Result of accuracy test

![Result_table](https://github.com/Rafalz13/Counting_objects/blob/master/images/result_table.png)



