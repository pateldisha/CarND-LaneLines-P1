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

My pipeline consisted of 5 steps. First, I converted the images to grayscale, then I am doing gaussian blur to the grayscaled image.
Then I applied canny edge detection algorithm to find the edges to the image. I divided the image using region of interest function to find only the required part.

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by finding the slope of the line. I used polyfit function for the same. 

Saved the output images in "test_images_output" folder and videos in "test_videos_output" folder.

If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image1]



### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be 


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to work on the challenge.mp4 video and finetune  the parameters such that it will work for such scenarios also. 

