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


## Training Data
<img width="734" alt="image" src="https://user-images.githubusercontent.com/117291117/228694252-33cb685d-7b71-42ce-886c-37205ed4e49e.png">
<img width="736" alt="image" src="https://user-images.githubusercontent.com/117291117/228694295-3b64b8d0-2fac-4165-8046-049b49d71282.png">
<img width="734" alt="image" src="https://user-images.githubusercontent.com/117291117/228694324-2f5d55ef-3c5a-49ad-b384-da48a7ca8a93.png">
<img width="733" alt="image" src="https://user-images.githubusercontent.com/117291117/228694360-1ee49ba0-081b-4d04-bb60-b85ea09c0d92.png">


## Testing Data
<img width="802" alt="image" src="https://user-images.githubusercontent.com/117291117/228693943-4bd80000-7124-4536-a31d-91cf8731b424.png">

<img width="801" alt="image" src="https://user-images.githubusercontent.com/117291117/228694040-ccb323f3-a86c-49c2-b488-8801d95a91c1.png">
