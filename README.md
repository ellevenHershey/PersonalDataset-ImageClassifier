<div align= "center"> 

  # Building a Custom Image Classifier with TensorFlow Using Personal Image Datasets from Google Drive
  A plant image classifier using Tensor Flow a project as a documented laboratory work to explore the efficacy of Convolutional Neural Network (CNN) on specialized image sets. 
  
  [Click here to visit Google Colab](https://colab.research.google.com/drive/1TshTi2eu0aI4xnN1MRUfeG-EhMsTddkR?usp=sharing)

</div>


## Dataset Preparation
#### How did you organize your dataset in Google Drive?
In my Google Drive, I first named a folder according to what plant family my datasets are, within that folder I made 20 different folders named to wht kind of plants my image sets are. After that I uploaded the images from my local storage into the drive.

#### Why is folder structure important for TensorFlow image loading?
In TensorFlow a structured folder is essential to automatically look at the folder names to know their class labels. If your pictures are in a different folder, the model might get confused or the model will fail. 

## Model Training 
#### What is the role of convolutional layers in image classification?
Convulational layer is like a filter that can scan an image to identify patterns, edges and colors. Essentially they transform raw pixels into recognizable feature that the computer can understand.

#### Why do we split data into training and validation sets?
We split data into a training set to teach the model patterns and unseen patern or pictures. This process ensures the model is actually learning to generalize rather than memorizing specific images.

## Performance Analysis
#### What accuracy did your model achieve? 
My model achieve accuracy: .36 in the validation 

#### How did the number of images affect the model's performance?
A larger number of images generally improved performance by providing the model with diverse examples to learn from. 

## Critical Thinking
#### What challenges did you encounter while using your own dataset?
Uploading different pictures took time then there goes training the model. It took very long time to get even 10 epochs. The plants who are very similar are also one of the challenges I encountered. 

#### How can data augmentation improve your model?
Data augmentation improved the model by making new versions of the images, it flipped or rotate the images. This makes the model better at recognizing the plants.

## Application
#### Suggest a real-world application for your trained model.
A practical real-world application for this model is for identifying plants when you are in the field. If this model is to be imporved and enhanced, like plant disease identifier would make a good real-world application. 

#### How can this system be integrated into a mobile or web application?
The model can be integrated by deploying the trained model TensowFlow Lite for mobile where user can upload images or take pictures using their cameras or using TensorFlow.js to run directly in browser. 

<div align="center"> 
  
  # Improving and Evaluating a Custom Image Classifier
  Enhancing Model Performance: Visualization, Overfitting Control, Data Augmentation, and Model
Deployment

</div>

## Visualization & Overfitting
#### What signs indicated overfitting in your first model?
The signs is the massive gap between the training accuracy (near 100%) and the validation accuracy (around 38%), combined eith a very high and unstable validation loss compared to a near-zero training loss.
#### How did data augmentation affect validation accuracy?
Data augmentation caused the validation accuracy to rise steadily alongside training, indicating that the model is now learning general features instead of just memorizing specific images.

## Model Improvement
#### What is the purpose of dropout layers?
Dropout layers randomly ignore a percentage of neurons during training which prevents the model from becoming over-reliant on specific patterns and it can now learn more generl robust features.  
#### Why does data augmentation improve generalization?
It creates artificial new image by flipping, rotating, or zooming on the images teaching the model that even upside the that the plant is still that plant.

## Performance Comparison
#### Compare accuracy before and after improvements.
Before improvement the model hit 100% training accuracy but only 38% validation accuracy, indicating severe memorization of the teaining dat. After applying data augmentation and dropout, both model is now learning actual visual features instead of memorizing only, making it more reliable for real-world use.
#### Which technique contributed most to improvement?
Data augmentation contributed the most because it directly addresses the lach of variety in the custom dataset. 

## Deployment & Application
#### Why is saving the model important?
Saving the model preserves the weights and architecture I have trained saving me time to not retrain everytime.
#### How can this model be deployed in a real-world system?
The model can be integrated by deploying the trained model TensowFlow Lite for mobile where user can upload images or take pictures using their cameras or using TensorFlow.js to run directly in browser. 
