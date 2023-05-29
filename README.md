# image_recognition_faces

## Face Recognition with PCA

We'll apply PCA to reduce the size of black & white images before applying classification algorithms:


Face Recognition

data: images of famous people
goal: compress images and use them as samples for a classification task

We will work on a dataset of multiple B&W images in order to find common patterns between all images in order to reduce the number of "principal features" that describe them!

More precisely, we will try to express each image of our dataset as a linear combination of principal components using PCA.

In order to compress our images, we will then zero-out the smallest principal components and keep only the most important ones in the equation.
Each "reduced linear combination" will represent an image that has been compressed.
(Because we only removed the least important components,) Our lower-dimensional projection of the dataset will preserve the maximal data variance between images, so we should still be able to recognize which person is in each image.



<img src="https://scikit-learn.org/stable/_images/sphx_glr_plot_face_recognition_001.png" width=500>
