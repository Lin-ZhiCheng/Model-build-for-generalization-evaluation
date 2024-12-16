# Model-build-for-generalization-evaluation
This repository is created to provide the code written in Pytorch for the paper 'A Generalisation Study in Deep Learning-based Segmentation of Lower-limb Muscles Across Different Populations' submitted to  Journal Scientific Report
# Code part

The png and label files hold the original MRI image and label as input, respectively. In this demo, the label contains 25 types of muscles, labelled from 1 to 25, with 0 representing the background. When you want to use your own data set, make sure that label is saved as a .png file and that each category is a positive number starting with 1. The number of classes in the last layer of the model is then adapted to the total number of classes plus 1, since background 0 is also a class considered in Pytorch.
In the main file is an example of the completed code, including data reading, preprocessing and modeling, and how to set hyperparameters in DL model training.
The example code uses 100 epochs, and it can be reserved to set the epochs from which the optimal model weight on the validation set is recorded. And the code will record the loss function of each iteration and the epoch's test set and validation set.
The Model file contains the pytorch encoding for the four models used in this article, namely U-Net[1], UNet++[2], Attention-UNet[3], and AFFU[4].


[1] O. Ronneberger, P. Fischer, and T. Brox, “U-Net: Convolutional Networks for Biomedical Image Segmentation,” arXiv, May 2015. Accessed: Dec. 05, 2023. [Online]. Available: http://arxiv.org/abs/1505.04597
[2] Z. Zhou, M. M. R. Siddiquee, N. Tajbakhsh, and J. Liang, “UNet++: A Nested U-Net Architecture for Medical Image Segmentation,” Jul. 2018, Accessed: Dec. 05, 2023. [Online]. Available: http://arxiv.org/abs/1807.10165
[3] O. Oktay et al., “Attention U-Net: Learning Where to Look for the Pancreas,” May 2018, Accessed: Dec. 05, 2023. [Online]. Available: http://arxiv.org/abs/1804.03999
[4] Z. Lin, W. H. Henson, L. Dowling, J. Walsh, E. Dall’Ara, and L. Guo, “Automatic segmentation of skeletal muscles from MR images using modified U-Net and a novel data augmentation approach,” Front. Bioeng. Biotechnol., vol. 12, p. 1355735, Feb. 2024, doi: 10.3389/fbioe.2024.1355735.
