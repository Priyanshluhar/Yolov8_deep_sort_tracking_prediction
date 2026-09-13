# Trajectory-Prediction-System

The primary objective of this project is to develop a comprehensive system for the accurate prediction of vehicle trajectories, with a particular focus on motorcycles, within a road environment. This undertaking encompasses three key components:

-><b>Vehicle Detection:<b/> <br>
Implementing advanced computer vision algorithms to identify and locate vehicles, specifically motorcycles, within video or image data streams. For this purpose I have chosen YOLOV8, whose source files can be found at https://github.com/ultralytics/ultralytics

-><b>Vehicle Tracking:<b/> <br>
Utilizing sophisticated tracking techniques to monitor and maintain the continuous identification and monitoring of vehicles as they move through the road scene.I have chosen DeepSort for this purpose. The required depedencies can be found at https://github.com/nwojke/deep_sort

-><b>Vehicle Trajectory Prediction:<b/> <br>
Employing predictive modeling methodologies to forecast the future paths and movements of vehicles, particularly motorcycles, based on their historical trajectories and current contextual data. I have Employed CNN-GRU and CNN-LSTM for this substep.<br><br> We give in the bounding boxes for 8 continuous frames of the tracked object, and the model predicts the next coordinate of the object based on these bounding box values. the Trained Models can be found in the Models Section of this repository. The code for training these models can be found at the Dataset and Training folder of the repository.

## Demo

https://github.com/Archangel0007/Trajectory-Tracking-System/assets/113388386/5dc8706b-3553-4aea-87bc-1c6184a2370a

You can see in the small demo. The center of every bounding boxes is the current state, the model is trying to predict the center point in the next state.
