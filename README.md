# Image Matching Challenge 2023
The competition task is: to reconstruct three-dimensional scenes through many different views. The process of reconstructing a 3D model of an environment from a set of images is called structure from motion (SfM).

And estimate the pose of each image in a set of N images. The pose of each camera has a rotation matrix R and a translation vector T as parameters from an arbitrary reference frame.

## Detection models:
**Keynet** is a deep learning model specifically for feature extraction. It uses a specific convolutional neural network architecture to extract keypoints and descriptors from the input image.

**GFTT (Good Features To Track)**  is a corner detection based feature extraction method mainly used for tracking "good" features in images. This method is based on the Shi-Tomasi method, which is an improved version of the Harris corner detection method. It finds N strongest corners in specified regions of an image.

**DoG (Difference of Gaussians)** DoG is a feature extraction method used in image processing by calculating the difference between images at different Gaussian blur levels. The resulting image has very high contrast, which highlights key features in the image. This method is often used in the Scale Invariant Feature Transform (SIFT) algorithm.

**Harris** Harris corner detection is a common image feature extraction method. It identifies features by measuring corners in an image. Corners are points where grayscale changes greatly in multiple directions, so they have good distinctiveness in images. The Harris method can still effectively detect corners after image transformations like rotation and scaling.
