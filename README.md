# car_detection
Car_detection_and_diraction_find
project containing the main code and progress done by me during the last year of my Bcs in electrical engineering
#date : 28.11.2024 
* finished the first part of creating a basic object finding based YOLOv8
* it was tested on the same val as train so not sure if it works
next to test on a bigger batch.

#python V1
from ultralytics import YOLO
import cv2
#load a model
model = YOLO("yolov8n.yaml") # build a new model

# use the model
results =model.train(data="config.yaml",epoch=2)
