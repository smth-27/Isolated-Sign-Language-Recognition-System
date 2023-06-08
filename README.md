# Isolated-Sign-Language-Recognition-System

About this project:

Isolated sign language recognition is crucial in improving accessibility and communication for the deaf and hard of hearing community, especially for babies born with permanent hearing loss. With the increasing number of such cases, there is a need for technological interventions that can help make learning sign language more interactive and accessible. In this paper, we propose the use of the TensorFlow Object Detection API for isolated sign language recognition using machine learning. The proposed system uses a convolutional neural network to detect and recognize sign language gestures.This technology has the potential to benefit the deaf and hard of hearing community by providing an alternative means of communication and connecting them with their loved ones.

Proposed System:

The proposed system aims to develop a real-time sign language detector using the TensorFlow object detection API. The system utilizes Python and OpenCV to capture images from a webcam and create a labeled map with 26 labels representing each alphabet in sign language. The training and testing data are used to generate TF records, which are used to train the TensorFlow object detection API.

For the object detection model, the system utilizes the SSD MobileNet v2 architecture with the FPN-lite feature extractor, shared box predictor, and focal loss. The training images are scaled to 320x320 pixels. The pipeline configuration is set up for transfer learning, allowing the model to incorporate prior knowledge of sign language to improve its performance. The model is trained for 10,000 steps, with hyperparameters controlling the number of steps and loss functions for classification, regularization, and localization.

Once trained, the model is loaded from the latest checkpoint and used for real-time sign detection using OpenCV and a webcam. The system detects signs in real-time and translates each gesture into English. The confidence rate of each detected sign is checked and tabulated for the final result.

The proposed system leverages the TensorFlow object detection API, which simplifies the development, training, and deployment of object detection models. Using TF records for data storage significantly improves the import pipeline's performance, reducing training time.

The real-time detection of sign language gestures enables efficient and effective communication between individuals who are deaf or hard of hearing and those who are not proficient in sign language. The system can be tested in real-time with different signs to ensure its accuracy and reliability in detecting and translating sign language gestures.

Overall, the system follows an algorithm that involves collecting and preprocessing data, training the SSD MobileNet v2 model using transfer learning, evaluating the model's performance, implementing real-time recognition, and continuously enhancing the system through user feedback and dataset improvements.


