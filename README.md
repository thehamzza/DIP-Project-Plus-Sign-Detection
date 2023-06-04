Image Pattern Locator

This Python code provides a simple and effective way to locate a specific pattern in an image and plot the coordinates of the pattern on the image. The code consists of two functions, locatePattern() and drawPoints(), both of which take an image file path as input.
Requirements

    Python 3.x
    OpenCV library
    Matplotlib library
    Numpy library

Installation

    Install the required libraries using pip install -r requirements.txt

Usage

    Import the code in your Python script using from image_pattern_locator import locatePattern, drawPoints.
    Call the locatePattern() function with the file path of the input image and an optional file path of the template image (if the template is not provided, the input image will be used as the template). The function returns the coordinates of the clustered points.
    Call the drawPoints() function with the file path of the input image and the coordinates of the clustered points returned by the locatePattern() function as input. The function plots the image and scatters the coordinates of the clustered points on top of it. The resulting plot is displayed.


Limitations

    The accuracy of the centers of the pattern may not always be true due to various factors such as lighting and contrast variations, thresholding errors, and the clustering algorithm used.
    The number of points was fixed to 8 because the KMeans clustering algorithm was used to group the points into clusters.

Acknowledgments

This code was developed based on the following resources:

    OpenCV documentation
    Matplotlib documentation
    Scikit-learn documentation


![sample image output](https://github.com/thehamzza/DIP-Project-Plus-Sign-Detection/assets/45312947/f9f310f6-9c8c-4705-80d4-5f8e74a875e3)

