# HARRIS Corner Detection

**Author**: Rachith Prakash

__Maintainer__ & __Contributer__: Rachith Prakash

Corner detection is a crucial process in Computer Vision. The corners are regions of large variations in intensity in the neighborhood of the point(pixel) in all directions. Thus, these are very good features to match between similar images.

This code is an example of Harris corner detection algorithm. I have included the code that compares the results with MATLAB's inbuilt harris corner detection algorithm.

NOTE: Remember to smoothen any image using a Gaussian filter before processing it.

This alogithm consists of following steps:

1. Smoothen image using a Gaussian filter.
2. Define filters to take derivatives (Prewitt, or Sobel).
3. Compute Gradient (derivatives) along x,y direction.
4. Compute the corner response measure for each pixel and compare it with a threshold value to categorize it as a corner/not a corner.
5. In order to get a clear output image, local maxima supression is implemented. In a 8-link window around each corner(pixel) detected from previous step, corners(pixels) having highest intensity in this neighborhood are retained. Others if any, are suppressed (zero intensity).

Reference: http://www.cse.psu.edu/~rtc12/CSE486/lecture06.pdf
