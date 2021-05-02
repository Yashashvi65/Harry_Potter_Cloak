# Working
First we start the webcam. And stores the starting frame in background variable.
After that we convert our normal RGB video frames to HSV so that we detect the color of the cloth.
After color detection we will get color range of our cloth.
We store lower values Hue, Saturation and Value in lower variable and higher values in upper variable. For making the mask.
Now we make mask. After that we open the mask and Dilate the mask.
Inverting the mask for front video frames.
Now masking the front video with 'inverted mask' and background frame with normal mask.
Adding both the result of video mask and background mask.
We will get the required output.
# Packages used:
-opencv-python 4.2.0.32
-numpy 1.19.1
