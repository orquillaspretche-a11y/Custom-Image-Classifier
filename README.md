# :file_folder: LW3_Custom-Image-Classifier

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

-The model achieved an accuracy of around 97% on the validation set. This shows that it was able to correctly classify most of the images and learned the important features needed to distinguish between the different classes.

:bulb: **How did the number of images affect the model’s performance?**

-The number of images affects the model’s performance because more images help the model learn better and recognize patterns more accurately. With too few images, the model may not perform well on new data.

**4. Critical Thinking**

:bulb: **What challenges did you encounter while using your own dataset?**

-During the initial model training, the main challenge I encountered was overfitting.  I implemented data augmentation and added dropout layers to the model, which are techniques designed to reduce overfitting and improve the model's generalization capabilities.
  
:bulb: **How can data augmentation improve your model?**

-Data augmentation helps the model by making more training images through small changes like flipping or rotating. This helps the model learn better and perform well on new images.

**5. Application**

:bulb: **Suggest a real-world application for your trained model.**

-A real-world application of my trained model is automatically identifying different plant or lettuce varieties in farms or gardens. This can help farmers quickly sort plants, monitor crops, and detect healthy or unhealthy plants without manually checking each one.

:bulb: **How can this system be integrated into a mobile or web application?**

-This system can be integrated into a mobile or web application by deploying the trained model on a backend server or using a lightweight version like TensorFlow Lite for mobile devices. The app can allow users to upload or capture images, send them to the model, and receive predictions in real time. Additional features like history tracking, notifications, or suggestions can also be added to improve usability. This makes it practical for farmers, students, or hobbyists to quickly identify plants, monitor crops, or classify objects directly from their phone or computer.

# :memo: Guide Questions (Student Reflection & Explanation) :memo:

:black_circle: **Visualization & Overfitting**

:bulb: **1. What signs indicated overfitting in your first model?**

-In the first model, overfitting was indicated by a divergence between training and validation metrics. Specifically, the training accuracy continued to improve, while the validation accuracy plateaued or slightly decreased. Concurrently, the training loss steadily dropped, but the validation loss began to increase after an initial decrease, signaling that the model was memorizing the training data rather than generalizing effectively.

:bulb: **2. How did data augmentation affect validation accuracy?**

-After implementing data augmentation and dropout, the validation accuracy of the model decreased. The initial model achieved a validation accuracy of 0.9684. The improved model, incorporating data augmentation and dropout layers, reached a validation accuracy of 0.7344 after 15 epochs. This decrease might be due to the regularization techniques, which aim to prevent overfitting but can sometimes lead to a slightly lower peak accuracy if applied too aggressively or if the original model was already robust on the validation set.

:black_circle: **Model Improvement**

:bulb: **3. What is the purpose of dropout layers?**

-Dropout layers are used in neural networks to prevent overfitting and improve how well a model generalizes to new data.

:bulb: **4. Why does data augmentation improve generalization?**

-Data augmentation improves generalization because it exposes the model to a wider range of input variations, helping it learn features that remain consistent across different conditions instead of memorizing specific examples.

:black_circle: **Performance Comparison**

:bulb: **5. Compare accuracy before and after improvements.**

-The validation accuracy of the model before improvements was 0.9684. After implementing data augmentation and dropout, the validation accuracy was 0.7344. While the original model achieved a higher validation accuracy, it also showed signs of overfitting. The improved model, with data augmentation and dropout, aims for better generalization, even if it results in a slightly lower peak validation accuracy on the specific validation set.

:bulb: **6. Which technique contributed most to improvement?**

-Data augmentation and dropout are generally techniques used to improve model performance and reduce overfitting. The validation accuracy of the improved model was 0.7344, which is lower than the initial model's accuracy of 0.9684. This suggests the goal was to improve generalization and mitigate overfitting, rather than achieve a higher peak validation accuracy.

:black_circle: **Deployment & Application**

:bulb: **7. Why is saving the model important?**

-Saving the model ensures your trained system can be reused, shared, deployed, and improved without starting over.

:bulb: **8. How can this model be deployed in a real-world system?**

-A model is deployed by connecting it to an application (web, mobile, or system) so users can input data and get real-time predictions.
