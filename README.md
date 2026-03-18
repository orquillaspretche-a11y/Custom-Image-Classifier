# :file_folder: Custom-Image-Classifier

**Google Colab link here:** https://colab.research.google.com/drive/1vD9SRjAGEZdKrmweM2M-kkufKxSchLQV?usp=sharing

# :memo: Guide Questions (Student Reflection & Explanation) :memo:

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

-The number of images affects the model’s performance because more images help the model learn better and recognize patterns more accurately. With too few images, the model may not perform well on new data.

**4. Critical Thinking**

:bulb: **What challenges did you encounter while using your own dataset?**

-One challenge I encountered was having insufficient or unbalanced images for some classes, which made it harder for the model to learn. Another issue was errors in file formats or corrupted images, which caused problems when loading the dataset. Organizing the images properly and making sure they were all usable took extra time.
  
:bulb: **How can data augmentation improve your model?**

-Data augmentation helps the model by making more training images through small changes like flipping or rotating. This helps the model learn better and perform well on new images.

**5. Application**

:bulb: **Suggest a real-world application for your trained model.**

-A real-world application of my trained model is automatically identifying different plant or lettuce varieties in farms or gardens. This can help farmers quickly sort plants, monitor crops, and detect healthy or unhealthy plants without manually checking each one.

:bulb: **How can this system be integrated into a mobile or web application?**

-This system can be integrated into a mobile or web application by deploying the trained model on a backend server or using a lightweight version like TensorFlow Lite for mobile devices. The app can allow users to upload or capture images, send them to the model, and receive predictions in real time. Additional features like history tracking, notifications, or suggestions can also be added to improve usability. This makes it practical for farmers, students, or hobbyists to quickly identify plants, monitor crops, or classify objects directly from their phone or computer.

# :memo: Guide Questions (Student Reflection & Explanation) :memo:

:black_circle: **Visualization & Overfitting**

:black_circle: **Model Improvement**

:black_circle: **Performance Comparison**

:black_circle: **Deployment & Application**



