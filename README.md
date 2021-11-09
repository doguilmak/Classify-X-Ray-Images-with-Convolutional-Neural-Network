
# Classify X-Ray Images with Convolutional Neural Network

## Problem Statement

The task at hand is to **classify diagnosis PNEUMONIA or NORMAL** using supervised machine learning method (CNN). Output layer is binary. Unfortunately, I couldn't put the images in the storage because the file size was too large. You can download the images from the[Kaggle](https://www.kaggle.com/paultimothymooney/chest-xray-pneumonia) webpage. After downloading, save the python file where the **chest_xray folder**.

## Dataset

Dataset has 5216 images belonging to 2 classes in total. **test** folder has 624 X-Ray images, **train** folder has 5216 X-Ray images and **val** folder has 18 X-Ray images.

**Example of NORMAL Class X-Ray Image:**

![normal_ex](Plot/normal.png)

**Example of PNEUMONIA Class X-Ray Image:**

![pneumonia_ex](Plot/pneumonia.png)

## Methodology

Within the classification study; there are two different results, in other words, two different output layer results such as PNEUMONIA or NORMAL. Since the study was carried out with a binary dataset, the trained model was compiled with **binary_crossentropy** loss function.

For understanding the methodology you are free to visit the [CNN Explainer](https://poloclub.github.io/cnn-explainer/) website. 

Converting CNN keras model (classifier) to dot format and save to a file:

![cnn_plot_model](Plot/binary_input_and_output_model.png)

val_accuracy:  **0.8845000267028809**

accuracy:  **0.82666665**

**Confusion Matrix**

| 1151 | 190 |
|--|--|
| **409** | **3466** |

Based on the trained model, predictions were made based on X-Ray photographs for the val file. 8  NORMAL class and 7 PNEUMONIA class X-Ray images used for the prediction . The results of the prediction can be seen in the following sequence.

  ***Prediction of NORMAL class:***
  
[[1.]]
[[0.]]
[[1.]]
[[1.]]
[[1.]]
[[1.]]
[[0.]]
[[0.]]

***Prediction of PNEUMONIA class:***

[[1.]]
[[1.]]
[[1.]]
[[1.]]
[[1.]]
[[1.]]
[[1.]]

***Took 250.25734400749207 seconds to classificate objects.***


## Contact Me

If you have something to say to me please contact me: 

 - Twitter: [Doguilmak](https://twitter.com/Doguilmak)  
 - Mail address: doguilmak@gmail.com
