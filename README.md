# ML Image Classification Project

This is a machine learning project where I created a custom image dataset and built essentially the same image classification model twice, once in PyTorch and once in TensorFlow.
I drew 260 images of various shapes to fall into four distinct categories: rectangles, ovals, triangles, and stick figures.

Each training set contained 60 images, while the testing set had 5 images (65 * 4 = 260).
After loading the data and preprocessing it, I built the learning model, ran through 15 training epochs, and then evaluated the results.

I compared my custom dataset to a separate control dataset from Kaggle (playing cards) so that I could be sure I was going through each step properly.

The full report can be found at the following link: https://chrisso.tv/pdf/ML_ImgClassificationReport.pdf

## Goals

- Learn more about Python and demonstrate an understanding of the basics of each ML library.
- Understand the differences in each step of the process between the libraries: loading data, preprocessing, building the model, training the model, and evaluating results.
- Be able to demonstrate that understanding with a detailed report that is accompanied by visualizations of key steps in the process.

## Outcomes  

After finishing this project, I definitely felt a stronger feel for how machine learning works. Previously, I had only used Scikit-Learn for linear/forest regressions, so jumping into an image classification project felt overwhelming at first. However, once I got past the loading/preprocessing phase in each library, the model and evaluation steps
felt somewhat intuitive. Some of the things I learned as I really dove into the subject matter:
- Model weights adjustments as well as forward/back propagation are informed by underlying calculus, meaning a neural network can be built with just the NumPy and Pandas libraries.
- The train/test split can be done manually or automatically in each ML library. I did it manually by loading the datasets from separate train/test directories.
- Randomization of the dataset to avoid bias can also be implemented in the preprocessing phase of each library (random rotation, colors, etc.). Before knowing this, I had already built my dataset with randomization in mind.

Once I finished, I definitely felt a stronger understanding of the differences in each library. TensorFlow gave me much more of a headache during the loading/preprocessing phase simply because I was adamant about getting my data loaded in with the same format as the MNIST dataset.
On the other hand, PyTorch felt more intuitive for loading/preprocessing data. Although it required more code to build the training loop, I did like how much more control I had in determining which metrics I wanted to pull as well as how I wanted to display them.

Overall, I definitely found myself gravitating towards PyTorch more than TensorFlow.
