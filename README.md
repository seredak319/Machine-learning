# Machine-learning MNIST dataset

## Goal
* Explore Azure Machine Learning Studio
* Comparison of learning methods
* Getting to know the basic tools for data analysis in Python
* Increasing the ability to work in a team

## Authors
[Krystian Sereda](https://github.com/seredak319)

[Martyna Skowrońska](https://github.com/martynaskowronska)

## Description
The project consisted in the classification of handwritten numbers using the MNIST database[1]. MNIST is the base
containing 70,000 handwritten digit images (10,000 being test data). Every image in the database is a 28x28 square.
Each pixel contained in the image is described for
using a number between 0 and 255 representing the gray scale. A value of 0 corresponds to an integer
black and 255 white. The aim of the project was to perform machine learning on a given set and
analysis of the obtained results.

## Exploratory analysis
The MNIST set contains 784 attributes describing each pixel in grayscale and
one decision attribute that assigns a handwritten number its true value.
In total, the collection contains 70,000 objects, 785 attributes and 10 classes (numbers from 0 to 9).
<p align="center">
<img width="204" alt="image" src="https://user-images.githubusercontent.com/95620581/221406050-1c7c3280-2d02-4739-8fc2-2a2828be22d9.png">

<img width="287" alt="image" src="https://user-images.githubusercontent.com/95620581/221406073-7ddcc381-0620-4634-ad23-df16f78564d8.png">
</p>

The examined set contains on average 7000 of each digit with the standard deviation not exceeding
6%. None of the classes significantly dominate the entire data set.
We considered the attributes that contained only 0 values and those that were strongly correlated as redundant. After
removing them, the number of attributes decreased to 711, which later affected the speed and
learning precision. The histogram below shows the changes made to the dataset.
<p align="center">
<img width="488" alt="image" src="https://user-images.githubusercontent.com/95620581/221406674-5228be25-856a-4b63-b264-ca150580c3c0.png">

</p>

### Averaged image of each digit
<p align="center">
<img width="485" alt="image" src="https://user-images.githubusercontent.com/95620581/221406418-eef0c074-1989-4527-8d50-159fbd82fee6.png">
</p>

### Averaged value of each digit
The average value of each digit, taking into account its content of white pixels.

<p align="center">
<img width="440" alt="image" src="https://user-images.githubusercontent.com/95620581/221406531-239cb70e-1e27-4c77-88c9-2ab02774a1fd.png">
</p>

### Randomly selected images

<p align="center">
<img width="467" alt="image" src="https://user-images.githubusercontent.com/95620581/221406642-c5279730-3218-428d-b845-6cb445fb4045.png">
</p>


## Results
The result contains a graph that allows to choose the best parameter for a given learning method and an Confusion matrix


### k-nearest neighbors
• Learing time: ~1.04s

• Precision: ~95%
<p align="center">
<img width="345" alt="image" src="https://user-images.githubusercontent.com/95620581/221407098-f4dcaf2c-a298-414d-87a6-a917a6087963.png">
<img width="302" alt="image" src="https://user-images.githubusercontent.com/95620581/221407100-c336bcc2-b009-4f15-b45e-08f2f98dada9.png">
</p>

### Decision tree
• Learing time: ~2.68s

• Precision: ~81%

<p align="center">
<img width="368" alt="image" src="https://user-images.githubusercontent.com/95620581/221407220-2678b297-2e91-4ca3-b21b-ce42f82a7ba9.png">
<img width="291" alt="image" src="https://user-images.githubusercontent.com/95620581/221407227-637132e5-5afe-445c-b489-a5ed5aa094ce.png">
</p>


### SVM
• Learing time: ~31s

• Precision: ~97%
<p align="center">
<img width="391" alt="image" src="https://user-images.githubusercontent.com/95620581/221407288-711f5bf1-d4fa-49ac-a317-7eda483a4235.png">
<img width="305" alt="image" src="https://user-images.githubusercontent.com/95620581/221407296-4b243d5b-960b-48bd-b313-f2427835c4c3.png">
</p>


### Test with our own number

<p align="center">
<img width="469" alt="image" src="https://user-images.githubusercontent.com/95620581/221407785-788fd6f8-bedc-4b54-ac8e-f1a3eb6f6201.png">
</p>

### Success :)

<p align="center">
<img width="325" alt="image" src="https://user-images.githubusercontent.com/95620581/221407812-e964d03f-4f78-4157-ab58-96f507e91caa.png">
</p>

## Sources
[1] https://en.wikipedia.org/wiki/MNIST_database
