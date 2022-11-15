# Unsupervised-Learning-Analysis-of-Transfer-Learning-Based-Features

1. I loaded the Keras model from keras.applications, pretrained on imageNet, that I used for transfer learning in the previous section, without the top layer.
2. I stacked a global average pooling 2D layer on top of this pretrained network.
3. I preprocessed the images from the testing portion of my transfer learning dataset and input all of them into this stack.
4. Then I performed PCA on the resulting series of feature vectors.
5. Finally, I generated a plot of the explained variance ratio versus number of dimensions kept under PCA.
