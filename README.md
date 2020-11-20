# Transfer Learning using InceptionV3 pre-trained model

## Transfer Learning
Transfer Learning is using a pre-trained model on a different but related problem. It will make use of the knowledge gained by the previous task to improve on the results of the current problem.Knowledge here is the weights at each layer of the model.
In transfer learning, we try to transfer as much knowledge as possible from the previous task the model was trained on to the new task at hand. This knowledge can be in various forms depending on the problem and the data.

![Transfer Learning](https://builtin.com/sites/default/files/styles/ckeditor_optimize/public/inline-images/classifiers-transfer-learning.jpeg)

In this Project, we are using pre-trained InceptionV3 model.

## InceptionV3 Model:
It is a convolution neural network that has 48 layers.This model has been pre-trained with millions of images from the ImageNet Dataset.The pre-trained InceptionV3 model can classify upto 1000 object categories.

![InceptionV3 Model Architecture](https://camo.githubusercontent.com/d93725579fc7e7140a60faadaaf47ae93eda84b6/68747470733a2f2f7777772e50657465724d6f7373416d6c416c6c52657365617263682e636f6d2f6d656469612f696d616765732f7265706f7369746f726965732f434e4e2e6a7067)

So, we have taken the the [Animal 10](https://www.kaggle.com/alessiocorrado99/animals10) Dataset from Kaggle which consist of around 28K medium quality animal images belonging to 10 categories: dog, cat, horse, spyder, butterfly, chicken, sheep, cow, squirrel, elephant out of which we are using only 500 images each of Dog and Horse.
The Dataset is unstructered, so we have first structured the Dataset using a user defined function. We are using the weights upto mixed7 layer of the INceptionV3 model after which we are adding a relu layer with 0.2 dropout and the after which the final layer has sigmoid as the activation function.
## Results
We are able to achieve a training accuracy of **94.33%** and a validation accuracy of **92.00%**
## References
1. **https://www.mathworks.com/help/deeplearning/ref/inceptionv3.html#:~:text=Inception%2Dv3%20is%20a%20convolutional,the%20ImageNet%20database%20%5B1%5D.&text=You%20can%20use%20classify%20to,using%20the%20Inception%2Dv3%20model**
2. **https://software.intel.com/content/www/us/en/develop/articles/inception-v3-deep-convolutional-architecture-for-classifying-acute-myeloidlymphoblastic.html#:~:text=Introduction,of%20Deep%20Learning%20Convolutional%20Architectures.&text=Inception%20V3%20was%20trained%20for,was%20a%20first%20runner%20up.**
3. **https://builtin.com/data-science/transfer-learning**
4. **Cousera - DeepLearning.AI TensorFlow Developer**
