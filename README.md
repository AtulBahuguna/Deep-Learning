# Deep-Learning
Auto-encoder project 

# Abstract
With the aid of this model, we will be able to extract data from partly or blurred photos and rebuild them. Using this approach to recognize people, cars, and other items is also highly helpful. Images that are important to a person or an organization today sometimes become blurry or have insufficient information. The CRL algorithm, also known as transfer learning, divides a data image into two parts, each of which may anticipate the other half of the data/image or create the data from the input. The aim of our model is to improve accuracy. As we use auto-encoder which is the two-phase operation of a neural network:
1.	A fixed-length vector is created from the input.

2.	Model reconstructs input from fixed encoded representation which is decodingphase.

For 2 channel autoencoder we use Corrent in which every channel represents a sperate view.


D ATA LOADING AND PRE- PROCESSING :

The images' left portions are stored in the file named leftdata-npy, and the right portions are stored in rightdata- npy. The labels associated with each pair are saved in the label file and will be used to evaluate transfer learning. To create training and testing sets, a custom split function was developed to divide the 2-view data into validation and training sets.

Using the split function, we can now prepare the training and validation datasets.
 
ENCODING PHASE :
In the encoding phase, we will utilize the Keras library to develop the Corrnet model. The encoding portion is established, and the Model branch creates an intermediate representation of the model that will be utilized during the decoding phase.

LAYERS IN KERAS :

In this section, we will develop certain custom layers using the Keras library to assist us in building the deep Corrnet model.

DECODING PHASE:

According to the Corrnet design utilized, four different types of losses were merged. To review these loss types, we will now look at the final cost function in the "Designing the Deep Corrnet" section.

RECOGNITION OF THE CONTRIBUTOR: Your choice of loss type will have an impact on how Corrnet is trained. Here, you may choose the batch size and iterations.

GENERATING IMAGES WITH CORRNET

![image](https://github.com/AtulBahuguna/Deep-Learning/assets/71915012/37cf7bc0-6803-4029-b5b6-1b24b3a68083)    ![image](https://github.com/AtulBahuguna/Deep-Learning/assets/71915012/b41495b5-15c1-4e96-8185-0fc3b5bbf50d)


# Motivation
We have seen a trend of blur in and incomplete image in recent years, which results in lack of information and can cause severe issues. For example, there is a hit and run case in the highway and a person clicks the photo of the car but somehow, he gets blur image in this case we can complete the image and can retrieve all the data required to find that person.

Transfer Learning has excited us to take this project because in transfer learning we can retrieve data from image and also, we can retrieve image from the data so we require only one parameter.

![image](https://github.com/AtulBahuguna/Deep-Learning/assets/71915012/9052c114-d4ca-4abd-ad93-c36a6b5ede1d)

# Output

![image](https://github.com/AtulBahuguna/Deep-Learning/assets/71915012/862ecd7e-496e-423c-9064-dded099b1d67)





![image](https://github.com/AtulBahuguna/Deep-Learning/assets/71915012/2a54e193-e015-4be2-8066-7c0ca18e16bd)

