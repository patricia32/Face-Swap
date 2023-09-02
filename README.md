# Face-Swap

This a simple Neural Network and Image Processing project for face swapping. I used a trained network that estimates the necessary parameters for the exchange and Jupiter to develop it. The library for the neural network is 'dlib' and I used it for face detecting and shape prediction.  

The implementation is simple and intuitive:
  - images reading
  - convert the images to grayscale
  - creating two empty masks
  - Steps for the first image
      - face detection and shape prediction
      - detect the face from the first image
      - facial references points are extracted
      - Delaunay transformation for triangles creation
      - extract the face and store the rest of the image in the mask
      - compute the indexes for triangulation
      - reconstruct the face using triangles and store it in the second image
  - repeat the steps to construct the face of the second image

![image](https://github.com/patricia32/Face-Swap/assets/125289158/c5b6a922-eacc-4fcf-9fc6-a8c3074a7092)
