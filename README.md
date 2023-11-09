# Scenario 1: Flower-Detection

In this project, I have tried to create a flower direction algorithm using deep learning I have taken the data set from Kaggle. This project has been developed to detect weather particular images at a flower or not.This can be further utilised in the big applications like flower captioning in which the customer can click the image of the flower and the customer will get the information about the flow.
## Kaggle Link
https://www.kaggle.com/datasets/alxmamaev/flowers-recognition/data
## Tools Used
- Google Colab
- Python
- Kaggle
- GitHub
- Laptop
- Internet
## Google colab link:
https://colab.research.google.com/drive/1haUrPrw5ijn-kmPWf8je3o3g_umOly4e?usp=sharing

## About Dataset
### Context
This dataset contains 4242 images of flowers.
The data collection is based on the data flicr, google images, yandex images.
You can use this datastet to recognize plants from the photo.

The pictures are divided into five classes: chamomile, tulip, rose, sunflower, dandelion.
For each class there are about 800 photos. Photos are not high resolution, about 320x240 pixels. Photos are not reduced to a single size, they have different proportions!

## Visualization
The given below file is the input. Here we can see the 5 tyes of flowers i.e. Daisy, Dandelion, Rose, Sunflower, and Tulips
![Flowers](https://github.com/AbhishekGit23/Flower-Detection/assets/123490715/718ad8e2-03d3-4857-b132-bbc6f4972dc7)

##Dataset Preprocessing 
Here I have applied the LabelEncoding as a Preprocessing. Also I have divided the Image by 255 to take it in the range of 0 to 1. As a greyscale image have values from 0 to 255.
![Screenshot 2023-11-09 102114](https://github.com/AbhishekGit23/Flower-Detection/assets/123490715/5354248e-238d-4b65-90dd-3afdef8b3131)

I have also used keras.preprocess.imge to process my images to prevent overfitting.
![Screenshot 2023-11-09 102123](https://github.com/AbhishekGit23/Flower-Detection/assets/123490715/5ed80bce-2d9a-488d-bf23-ede9704e70c7)

## Modeling 
- For modeling my data I have used CNN ie Convolutional Neural Network. with 40 filters and ReLu as my Activation Function.
- Then I have applied Max Pooling 2D to reduce the size and resolution of the image with pool size as 2X2.
- Then again I have applied the convolutional layer with 50 filters and activation function as ReLu.
- Then again I have applied MaxPooling2D with pool size as 2X2 and here I have also applied the strides as 2X2 so that less feature reduction will be there.
- Then again I have applied the convolutional layer with 55 filters and activation function as ReLu.
- Then again I have applied MaxPooling2D with pool size as 2X2 and here I have also applied the strides as 2X2 so that less feature reduction will be there.
- THen again I have applied the convolutional layer with 60 filters and activation function as ReLu.
- Then again I have applied MaxPooling2D with pool size as 2X2 and here I have also applied the strides as 2X2 so that less feature reduction will be there.
- Then I have applied the flatten layer.
- Lastly I have applied 4 Dense Layers aith size 100, 200, 200 and 100. Here also I have used ReLu as my Activation Function.
- Then the final Dense layer with 5 size and here I have used SoftMax as ny Activation Function. This layer will give 10 possible classes of flowers.
![Screenshot 2023-11-09 102206](https://github.com/AbhishekGit23/Flower-Detection/assets/123490715/9a042396-c017-4f91-9940-2b5dd05a76a1)

## Model Summary
![Screenshot 2023-11-09 102215](https://github.com/AbhishekGit23/Flower-Detection/assets/123490715/bc7573b0-7028-450d-94a6-430e01cc3fb2)


## Fitting Nodel
For futting the model I have used batch size as 128, number of epochs as 50, and verbose as 1.
![Screenshot 2023-11-09 102344](https://github.com/AbhishekGit23/Flower-Detection/assets/123490715/c269d2fa-9e30-4904-a5f1-4e4fa15729d1)
![Screenshot 2023-11-09 102330](https://github.com/AbhishekGit23/Flower-Detection/assets/123490715/14fa7e6f-abde-4516-a289-e338f1a266c5)


## Graphs
### Comparision of Loss of Training and Testing Data VS No. of Epoches
![Graph3](https://github.com/AbhishekGit23/Flower-Detection/assets/123490715/7149a858-3adc-435c-bd71-734ace372dbc)

### Comparision of Model Accuracy of Training and Testing Data VS No. of Epoches
![Graph4](https://github.com/AbhishekGit23/Flower-Detection/assets/123490715/a8077431-e278-4264-8b88-289c20f4a68f)

## Conclusion 
In the last I will conclude by giving the model loass and accuracy as 0.7966 and 0.785 respectively also the validation loass and validation accuracy as 0.8198 and 0.7157 respectively.
![Screenshot 2023-11-09 102423](https://github.com/AbhishekGit23/Flower-Detection/assets/123490715/5f1e4908-56ee-4b0b-ada5-d4fa45b4709c)

So, this is the project which I have developed. Hope you liked it.
