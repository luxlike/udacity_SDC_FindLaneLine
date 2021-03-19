# **Finding Lane Lines on the Road** 

---

**Finding Lane Lines on the Road**

The goals / steps of this project are the following:
* Make a pipeline that finds lane lines on the road
* Reflect on your work in a written report


[//]: # (Image References)

[image1]: ./test_images/solidWhiteCurve.jpg "Original image"
[image2]: ./test_images_output/gray_solidWhiteCurve.jpg "Gray scale image"
[image3]: ./test_images_output/blur_solidWhiteCurve.jpg "Gaussian blur image"
[image4]: ./test_images_output/canny_solidWhiteCurve.jpg "Canny edge image"
[image5]: ./test_images_output/roi_solidWhiteCurve.jpg "ROI image"
[image6]: ./test_images_output/hough_solidWhiteCurve.jpg "Hough line image"
[image7]: ./test_images_output/weighted_solidWhiteCurve.jpg "Weighted image"

---

### Reflection

### 1. Describe the pipeline

My pipeline consisted of 6 steps.(Defined in process_image function)

1. Step one

Apply the gray scale transform using grayscale() function

In order to draw a single line on the left and right lanes, I modified the draw_lines() function by ...

If you'd like to include images to show how the pipeline works, here is how to include an image: 

![alt text][image1]

![alt text][image2]

2. Step two

Apply the gaussian blur effect using gaussian_blur() function

![alt text][image3]

3. Step three

Apply the canny edge using canny() function

![alt text][image4]

4. Step four

Define ROI(region of interest) with vertices using region_of_interest() function

![alt text][image5]

5. Step five

Draw hough lines using hough_lines() function

![alt text][image6]

6. Step six

Finally, weight hough line to original image.

![alt text][image7]


### 2. Identify potential shortcomings with your current pipeline


One potential shortcoming would be what would happen when ... 

Another shortcoming could be ...


### 3. Suggest possible improvements to your pipeline

A possible improvement would be to ...

Another potential improvement could be to ...
