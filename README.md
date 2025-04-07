# Hand Image Clustering with Manual K-Means

This project demonstrates unsupervised image segmentation by manually implementing the K-Means clustering algorithm from scratch. The input image contains multiple hand instances, and the algorithm groups pixels into clusters based on their RGB values to segment different regions of the image.

## Project Overview

- Type: Unsupervised Machine Learning
- Goal: Segment an image with hands into distinct regions using clustering
- Algorithm: K-Means Clustering (implemented manually)
- Input: RGB image containing multiple hand visuals
- Output: Clustered image showing pixel groupings

## Key Features

- Full manual implementation of the K-Means algorithm
- Image reshaping and preprocessing using NumPy
- Visualization of original and clustered images using matplotlib
- No use of external ML libraries like scikit-learn for clustering

## K-Means Algorithm Steps

1. Flatten the image into an array of pixels with RGB values.
2. Randomly initialize `k` centroids (each centroid is a 3D RGB point).
3. Repeat until convergence or for a set number of iterations:
   - Assign each pixel to the nearest centroid based on Euclidean distance.
   - Recompute each centroid as the mean of the pixels assigned to it.
4. Map each pixel to its centroid’s color to create the segmented output image.

## Skills Demonstrated

- Understanding of unsupervised learning principles
- Algorithmic thinking through step-by-step implementation
- Efficient manipulation of image and matrix data
- Visual interpretation of clustering results

## Technologies Used

- Python
- NumPy
- Matplotlib
- OpenCV (optional, for image reading)

## How to Run

1. Clone this repository
2. Install dependencies:
   ```bash
   pip install numpy matplotlib opencv-python
