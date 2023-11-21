# CV_FaceSwapping
face swapping in python using opencv, mediapipe, and other tools.

This code is an implementation of face swapping using OpenCV in Python. It reads two images, detects facial landmarks in each image, and then swaps the faces in the images. The code uses the Delaunay triangulation algorithm to find corresponding triangles in the two images, and then applies an affine transformation to each triangle to warp the triangles from one image to the other. Finally, the code blends the two images together to create a seamless face swap.

In the code with hand-written points, the code starts by importing the necessary libraries, including sys, numpy, and cv2. It then defines several functions, including readPoints, applyAffineTransform, rectContains, calculateDelaunayTriangles, and warpTriangle. These functions are used to read the facial landmarks from a text file, apply an affine transformation to a set of points, check if a point is inside a rectangle, calculate the Delaunay triangulation of a set of points, and warp a triangular region from one image to another.

The main function of the code starts by checking the version of OpenCV being used. It then reads two images and the corresponding facial landmarks from text files. The code finds the convex hull of the facial landmarks in each image and calculates the Delaunay triangulation of the convex hull points. It then applies an affine transformation to each triangle in the Delaunay triangulation to warp the triangles from one image to the other. Finally, the code blends the two images together to create a seamless face swap and displays the result.

In the code using Mediapipe face mesh detector, it's somehow the same, with difference being that the points are obtained using mediapipe face mesh detector, that gives landmarks as its result and the face is completely affined on the source image.

with help from:
1. https://learnopencv.com/face-swap-using-opencv-c-python/
2. Mediapipe demos: face mesh
3. https://youtu.be/gthvlYTAuqI?si=f3LfMqKlU75wamsg
...
