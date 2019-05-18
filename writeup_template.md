# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./examples/grayscale.jpg "Grayscale"
[image2]: ./test_images_output/solidWhiteCurve.jpg "Solid white curve"

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My pipeline consisted of 5 steps. 
  - I converted the images to grayscale
  - I applied Gaussian smoothing module
  - I used Canny edge detection
  - I have selected the region of interest
  - I applied Hough Transform line detection
  - I combined images

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by getting the lines's slope

If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image2]


### 2. Identify potential shortcomings with your current pipeline


This image processing could maybe be faster 


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to handle curved line like in the challenge part
