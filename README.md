# Tracker-v1

## Setup your own envirement using VScode

Open the Command Palette (Ctrl+Shift+P), search for the Python: Create Environment command, and select it. 
The command presents a list of environment types: Venv or Conda. Use Venv

Next your gonna want to install tensorflow, tensorflow_hub, ect, use

!pip install tensorflow==2.4.1 tensorflow-gpu==2.4.1 tensorflow-hub opencv-python matplotlib

Now you are able to run the multipose model





## FUTURE PLANS


1. **Data Collection**: Gather a dataset of images that contain the big circle (plate) on a barbell in various positions and orientations. The dataset should also include corresponding annotations for the center of the circle in each image.

  - From now on every time we squat, bench or deadlift we need to be recording with a side view, use different color plates at the end and switch clothes up
  - files are in the github,


2. **Data Preprocessing**: Preprocess the images and annotations to bring them into a suitable format for training the model. Common preprocessing steps include resizing, normalization, and augmentation.

  - Use transfer learning: If you have a limited dataset, you can use transfer learning by starting with a pre-trained model (e.g., from the TensorFlow Object Detection API) and fine-tuning it on your specific dataset.
  - Use annotated data: Make sure that your dataset includes annotations for the center of the big circle in each image. These annotations will be essential for training the model and tracking the circle's movement.  
    ** For this use https://www.youtube.com/watch?v=-ZyFYniGUsw

3. **Model Selection**: Choose a suitable deep learning architecture for the image recognition task. You can start with a pre-trained object detection model or use a custom architecture like a Convolutional Neural Network (CNN) for this specific task.
    
4. **Model Training**: Train the chosen model on the preprocessed dataset. During training, the model learns to recognize and locate the big circle in the images.
    
5. **Testing and Evaluation**: Evaluate the trained model on a separate test dataset to assess its performance. Measure metrics such as accuracy, precision, recall, and F1-score to gauge the model's effectiveness.
    
6. **Object Tracking**: To track the middle of the circle as it moves, you'll need to implement an object tracking algorithm. There are several methods available, such as Kalman filters, optical flow, or deep learning-based approaches like SORT (Simple Online and Realtime Tracking).

  ** Need to learn this, not sure whats going on here.
    
7. **Deployment**: Once the model and tracking algorithm are working satisfactorily, integrate them into a real-time system or application that can process live video streams or image sequences from a camera.
    
  ** For this we will use swift to integrate within a application, using ios to start
  ** Will need Xcode, this will be probably 60% of the learning,


Here are some additional tips:

    
- Consider real-time constraints: If you want the model to perform real-time tracking, ensure that your chosen architecture is efficient enough for fast inference on the target hardware.
    
- Regularly update the model: If you are building a tracking system for a dynamic environment (e.g., a gym), consider updating the model periodically with new data to adapt to changes in lighting conditions, backgrounds, and other factors.
    

Building an image recognition and tracking system can be a complex task, so it's essential to have a good understanding of deep learning, computer vision, and object tracking concepts. Depending on your experience, you might want to seek help from experienced researchers or developers in the field.



The goal is to create a software good enough that we could potentialy sell to gymshark or another big name gym company,



