## Learn Hand Written Characters using Probability

Given a set of 100 4x4 pixel images containing only 0s and 1s, let X = {X[1], X[2],...,X[16]} be the pool of all possible images. Let Y = {Y[1], Y[2],...,Y[16]} be a new input image. 

This code seems to implement a Naive Bayes classifier to recognize handwritten digits 0 and 1. The code loads images of handwritten 0's and 1's, creates a binary matrix representation of each image, and counts the number of times each pixel is set to True (ink is present) for each digit. It then calculates the probability of each pixel being True given the digit is a 0 or 1, and uses these probabilities to classify a new input image as a 0 or 1.

Specifically, the code:
- Loads all the images of handwritten 0's and 1's from a specified directory 
- Creates a binary matrix of size 4x4 for each image 
- Goes through each matrix and counts the number of times each pixel is set to True for each digit 
- Uses the count to calculate the probability of each pixel being True given the digit is a 0 or 1

Next, the code:
- Loads a new image 
- Creates a binary matrix representation of it 
- Compares each pixel to the probabilities calculated earlier to determine whether the input image is more likely to be a 0 or 1 
- Calculates and prints out the probability of the input image being a 0 or 1
