# **Finding Lane Lines on the Road** 

## Writeup Template

### You can use this file as a template for your writeup if you want to submit it as a markdown file. But feel free to use some other method and submit a pdf if you prefer.

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report

Delivarables
* Code for the project is in P1.ipynb
* Video output
  1. [Solid white right](./output/test_videos_output/solidWhiteRight.mp4)
  2. [Solid yellow lefy](./output/test_videos_output/solidYellowLeft.mp4)

---

### Reflection

### 1. Describe your pipeline. As part of the description, explain how you modified the draw_lines() function.

My Pipeline is explained in the series of steps below with intermediate images for those steps.

1. Gray Scale Conversion
2. Gaussian smoothing
3. Canny Edge detection
4. Masking Interesting polygon region
5. Hough transform
6. Draing annotated images

![alt text][image1]


### 2. Identify potential shortcomings with your current pipeline

1. Does not work well when we are travelling around the curves. Lane lines are curved
2. Is very much dependent on lane width since we mask regions using hard coded parameters
3. 


### 3. Suggest possible improvements to your pipeline

1. Possibly 