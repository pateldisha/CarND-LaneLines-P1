# **Finding Lane Lines on the Road** 

## Writeup

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Making a pipeline that finds lane lines on the road



[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of below steps. 
First, I converted the images to grayscale, then I am doing gaussian smoothing to the grayscaled image.
Then I applied canny edge detection algorithm to find the edges to the image.

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by finding the slope of the line. I used polyfit function for the same. Then created the line from top to bottom.

Saved the output images in "test_images_output" folder and videos in "test_videos_output" folder.



### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when we try to apply it to challenge.mp4 video which is having turning in the lane lines.


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to make the pipeline work on the challenge.mp4 video and finetune  the parameters such that it will work for such scenarios also. 

