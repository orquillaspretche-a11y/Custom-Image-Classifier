# Custom-Image-Classifier

**Google Colab link here:** https://colab.research.google.com/drive/1vD9SRjAGEZdKrmweM2M-kkufKxSchLQV?usp=sharing

# :memo: Guide Questions (Student Reflection & Explanation)

**1. Dataset Preparation**

:bulb: **How did you organize your dataset in Google Drive?**

-I organized my dataset in Google Drive by creating a main dataset folder with subfolders for each image class.

Dataset

├── Class_1 (e.g., Arugula_Lettuce)
│   ├── img1.jpg
│   ├── img2.jpg
│

├── Class_2 (e.g., Batavia_Lettuce)
│   ├── img1.jpg
│   ├── img2.jpg
│

├── Class_3 (e.g., Buttercrunch Lettuce)
│   ├── img1.jpg
│   ├── img2.jpg
│

:bulb: **Why is folder structure important for TensorFlow image loading?**

-The folder structure is important because TensorFlow automatically assigns labels based on the folder names when loading images.

**2. Model Training**

:bulb: **What is the role of convolutional layers in image classification?**

-Convolutional layers help extract important features from images such as edges, textures, and shapes. They use filters to scan the image and detect patterns that help the model understand what is in the image. These features allow the system to recognize and correctly classify different images.

:bulb: **Why do we split data into training and validation sets?**

-We split data into training and validation sets so the model can both learn and be evaluated properly. The training set is used to train the model and allow it to learn patterns and features from the images. The validation set is used to check how well the model performs on data it has not seen before. This helps measure the model’s accuracy and ensures that it can generalize to new images instead of just memorizing the training data, which helps avoid Overfitting.

**3. Performance Analysis**

:bulb: **What accuracy did your model achieve?**

-The model achieved an accuracy of around ___% on the validation set. This shows that it was able to correctly classify most of the images and learned the important features needed to distinguish between the different classes.

:bulb: **How did the number of images affect the model’s performance?**

**4. Critical Thinking**

:bulb: **What challenges did you encounter while using your own dataset?**
  
:bulb: **How can data augmentation improve your model?**

**5. Application**

:bulb: **Suggest a real-world application for your trained model.**

:bulb: **How can this system be integrated into a mobile or web application?**





