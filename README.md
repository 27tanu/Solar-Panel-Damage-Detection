# Solar-Panel-Damage-Detection
This project is a deep learning-based solution to detect damage in solar panels using object detection models. We implemented various versions of the YOLO (You Only Look Once) model, including YOLOv5, YOLOv7, YOLOv8, and YOLOv9, to identify defects in solar panels, with images annotated using Roboflow.

Table of Contents

•	Introduction
•	Features
•	Data Collection and Annotation
•	Models Used
•	Usage
•	Results
•	Deployment
•	Screenshots of detection
•	Future Improvements
•	Acknowledgments

1.	Introduction
The goal of this project is to accurately detect various types of damages in solar panels, including dusty, physical damage, electrical damage, bird droppings, and more. Early detection of such issues can help in maintaining solar panel efficiency and preventing further deterioration.

2.	Features
Multi-class damage detection ('Bird-drop', 'Clean-Panels', 'Defective', 'Dusty', 'Electrical-Damage', 'Physical-Damage')
Implementation using multiple YOLO model versions for comparative analysis
Real-time and batch detection capabilities
Annotation management with Roboflow

3.	Data Collection and Annotation
The dataset used in this project consists of annotated images of solar panels, categorized by damage type. Roboflow was used to annotate the images for consistent, high-quality annotations. The dataset is organized into three folders:

Train: For training the YOLO models
Validation: For validating the models during training
Test: For evaluating model performance

4.	Models Used
We utilized four versions of the YOLO model to compare performance:

YOLOv5
YOLOv7
YOLOv8
YOLOv9

Each model's performance was evaluated using Mean Average Precision (mAP) and inference time to identify the most suitable model for the task.


5.	Results
We compared the results across YOLOv5, YOLOv7, YOLOv8, and YOLOv9 models, using metrics such as:

mAP@0.5: Evaluates model accuracy at 50% IoU
mAP@0.5:0.95: Average precision across multiple IoU thresholds for a more robust evaluation
Inference time: Measured the speed of each model for real-time use cases
Detailed performance results are included in the results folder.

6.	Deployment
Deployed using Streamlit.
![image](https://github.com/user-attachments/assets/92caa9d6-8978-4a4c-a5ce-1622fc5109a4)

 

7.	Screenshots of Detection
 ![image](https://github.com/user-attachments/assets/1b6a4476-fbf6-45e6-b834-18af244f037d)

![image](https://github.com/user-attachments/assets/5deda1af-7855-4176-92a0-f38cd29694d2)
![image](https://github.com/user-attachments/assets/c747cf7c-2fbd-4365-b160-afd24ab73c72)


 

 
 



8.	Future Improvements
Enhance the dataset with more diverse damage types and weather conditions.
Experiment with advanced post-processing techniques to improve detection accuracy.
Explore real-time deployment options on edge devices.
9.	Acknowledgments
Special thanks to Roboflow for providing an intuitive annotation tool, and to the developers of YOLO models for their powerful object detection frameworks.
