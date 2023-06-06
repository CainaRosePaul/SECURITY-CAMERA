# SECURITY-CAMERA


The code initializes the camera using OpenCV and captures frames in a loop. It calculates the difference between consecutive frames and converts it to grayscale. A Gaussian blur is applied to reduce noise, followed by thresholding to create a binary image. The binary image is further processed through dilation and contour detection.

Contours with an area less than 5000 are ignored, while larger contours are identified as potential motion areas. These areas are outlined with rectangles on the frame, and a sound effect is played using the winsound library.

The system continues detecting motion until the 'q' key is pressed, at which point the program terminates. The camera feed with motion detection overlays is displayed in a window titled "Granny cam."


