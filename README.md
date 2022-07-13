# LICENSE PLATE DETECTOR

A simple model for license plate detection. The main goal of the project was to learn how to train YOLOv5 on a custom dataset.

# WORKFLOW
## YOLOv5 model training

First, I familiarized myself with how data is labeled and how to YOLOv5 network model is trained ([link_1](https://blog.paperspace.com/train-yolov5-custom-data/amp/), [link_2](https://blog.roboflow.com/how-to-train-yolov5-on-a-custom-dataset/?ref=ultralytics)). Then I searched for some images. I found a collection with ready-made labels ([dataset](https://www.kaggle.com/datasets/andrewmvd/car-plate-detection)), just needed to change the data format from XML to one that YOLOv5 network accepts. The entire process can be found here: model/yolov5_training. The result can be seen below:

![results](https://user-images.githubusercontent.com/76869717/178729030-bbd468f4-ec9f-4c39-8fb0-7edc0bcb1c91.png)

## Playing around with the detect.py file

Finally, I checked what I could do with the detected objects. I decided to blur the detected license plates (as in the image below).

![res](https://user-images.githubusercontent.com/76869717/178738179-5e82b5af-0d82-468f-a041-89fdbd46c598.png)
