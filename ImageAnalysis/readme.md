# Image Processing and Analysis in the health area

**This project covers the basics of image processing and analysis for the extraction of meningful data; then we will see an example of how to detect a tumor in the lungs.**

## What is it about?

The jupyter notebook will cover the basics of processing and modifying an image by performing various operations to observe anomalies and extract information, this to put the theory into practice. First, a drawing of a head from different angles will be dealt with, and then it will be with an x-ray radiography for the detection of a tumor in the lungs. So let's start with the theory.

## How does a computer process an image?
A computer sees an image as a two-dimensional array, where one is the **height** and the other the **width**, so if the image is 1080 x 1920 pixels, the computer will handle a matrix of [1080][1920] elements, where each element is a pixel. 

But now **How does a computer handle a pixel?**
A computer treats a pixel as an vector or list of **3 values**, where each value is the intensity of the pixel in red, green and blue, that is its *RGB* values. 

In summary, a computer treats an image as a 2-dimensional array specifically arranged in rows and columns, where each value is a vector of 3 elements. Knowing this we can change the color of the pixel we want, we only need to know its exact position in the image and its new RGB values; but changing a pixel will not modify the image significantly, so here comes the **Color Image Processing**.

## Image Color Processing 

Is about how we can change the color of the pixels to focus on certain points or make certain parts of the image stand out to get more information; to control this part we have to know the basics of RGB color theory, for example if we want to make the image in grayscale we have to make the 3 RGB values equal. Many times we will only be interested in one part of the image and therefore we will only want to modify that part, so for this we must **segment the image**, which is another basic aspect of image processing.

## Image segmentation

This involves **in dividing an image into regions or segments**, each of which corresponds to a specific **object or feature** in the image. For example, if you are processing images of butterflies to find patterns in their wings, you only want to process the wings and not their body or background, so you segment the image to focus only on their. Then, when the image is segmented, it is necessary to give more clarity to those areas, so enhancement techniques are now used.

## Image enhancement 

This involves **improving the visual quality** of an image, such as increasing contrast, reducing noise, and removing artifacts. Once we do this we can finally do the object detection techniques.

## Object Detection and Recognition

This is finding shapes or patterns in the image to extract information, after having done all the above techniques, this can be simplified or automated with machine learning.

### And then what?

Image Processing and Analysis has many more areas, models and treatments for obtaining information or modifying images, remember that this is only the basics; there is still something very important missing that is of great help for this area **Machine Learning and Artificial Intelligence**.