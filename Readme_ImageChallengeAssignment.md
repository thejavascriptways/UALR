# Image Challenge Assignment
For this assignment, we have posted several challenge ideas for working with images. 
For this week's assignment, you can pick one of the attached sheets and try your hand at how you might solve the tasks 
listed for a particular project page using tools, techniques, or algorithms that you can find on the web.


In addition to providing the input and output (results), you also need to write up your findings as a short report, 
explaining how you tackled the tasks or challenge listed in that Project (i.e., provide the code/steps that you used to complete the assignment. 
Note: You are also welcome to use this assignment as inspiration for developing these project tasks (or something like these project tasks) into 
a full-blown data science term project/paper and presentation for this course.


## Project_ImageProcessing.pdf

Project : Implementation of image processing
operations
In this project, you'll be expected to write a bunch of image processing operations. You are
expected to write a report with the results included in the report. You must include in the
report your original and filtered images and a description of what your filter does.
You can handle the boundary conditions by ignoring the first and last rows and the first and
last columns in the output image. Feel free to use any software or programming environment
of your choice, like Matlab.
Your Tasks:
The first task needs a color image and all the other tasks need greyscale images. You can
generate the greyscale images using GIMP or a similar tool, by saving the image with the
extension png.
1. Black and white
Write a filter that converts a color image to black and white. Simply take the average of the
colors and save as the Red, Green, and Blue values in the result. Note that the output is still a
color image, but it has B&W content.
2. Gaussian filter
Build and implement a 7x7 Gaussian filter
3. Thresholding
Generate the histogram of the image using GIMP, and then select one value as a threshold.
All pixels with luminance greater than the threshold become white, all below become black.
4. Prewitt derivative estimate
Implement two filters that do the Prewitt derivative estimate operators. The horizontal
operator is:
-1 0 1
-1 0 1
-1 0 1
The vertical version is:
-1 -1 -1
0 0 0
1 1 1


## Project_Retrieval.pdf
Project: Multimodal Content Retrieval
In this project, you are going to design and implement algorithms that
demonstrate the impact of multimodal analysis and searching of multimedia
data.
Create a sample collection of social media-based images with associated
captions, tags, paragraphs etc.
Implement a text-based searching method that allows a user to retrieve
images based on the matching of search keywords with the text associated
with the image. For example, search for images with trees using the keyword
“tree” or similar words and look for full or partial matching of the keywords
in the text related to an image.
Implement an image search and retrieval method using visual features like
color, shape, contour etc.
Implement a combined, multimodal search and retrieval method that utilizes
both text and image based matching mechanisms.
Prepare a comprehensive report of your findings, including the precision and
recall comparisons of text, image, and multimodal retrieval methods for a set
of selected queries, such as “find images with trees” The report should
underline any significant improvement multimodal retrieval offers over the
monomodal mechanisms, if any.
BONUS: Extend the multimodal retrieval mechanism to video data, using
representative frame idea or a similar mechanism to reduce the complexity
of the search space of your data.
To test and implement your algorithm, you can use Matlab or any alternative
programming language/platform. As an input your algorithm can accept
common image formats, .avi files or any other common video format.
Reference Materials:



## Project_CutDetection.pdf

Project: Scene Cut Detection
Design and implement an alternate algorithm to detect the scene cuts in a
video clip. Compare your method with the histogram-based algorithm
described below.
To test and implement your algorithm, you can use Matlab or any alternative
programming language/platform. As an input your algorithm can accept .avi
files or any other common video format.
Histogram-based cut detection
H(f,i) is the histogram value at bin i. This formula is used to compute the histogram-
based dissimilarity between any two consecutive frames.
Algorithm steps:
Read AVI file and store each frame as a “bmp” image.
Histogram-based image dissimilarity
Read each frame as a bitmap
Convert to gray-scale bitmap
Compute histogram for each frame
Apply the above formula to compute the difference
Store the difference in the output array
Find frames - histogram-based dissimilarity
Accept output array from histogram-based image dissimilarity
Compute the threshold value: average between max and average
Find frames that are above the threshold value
Plot output, compute the number of cuts.( ) ( )
=
−=
255
0
2
))(())(()(),( i
igHifHgHfHd


