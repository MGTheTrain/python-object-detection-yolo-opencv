# object-detection-yolov3-opencv

## References 

- [darknet Github repository](https://pjreddie.com/darknet/yolo/)
- [yolov4_darknet Github repository](https://github.com/kiyoshiiriemon/yolov4_darknet)
- [YOLO: Real Time Object detection](https://pjreddie.com/darknet/yolo/). The tutorial also explains how unsupervised learning can be applied for the YOLO architecture to generate a trained model (`weights` (weights of the nodes determined by backward pass), `cfg` (the actual CNN) and `<obj/coco>.names` (file containing the classes utilized for training in a text file) file).

## How to use

#### Perequisite

Python release version 3.9, 3.10 or 3.11. 

#### Install the pip packages

```sh
pip install -r requirements.txt
```

#### Retrieve files for required for model inference (in this case object-detection)

Following links can be utilized to download the `.weights` files:

- [yolov3.weights](https://pjreddie.com/media/files/yolov3.weights)
- [yolov3-tiny.weights](https://pjreddie.com/media/files/yolov3-tiny.weights)
- [yolov4.weights](https://github.com/AlexeyAB/darknet/releases/download/darknet_yolo_v3_optimal/yolov4.weights)
- [yolov4-tiny.weights](https://github.com/AlexeyAB/darknet/releases/download/darknet_yolo_v4_pre/yolov4-tiny.weights)

Copy those weights in the `cfg` folder in this project.

**(Optional since files already exist in the cfg and object-names folder)** Following steps shall be considered in order to retrieve the`.cfg` and `.names` (list of classes) files:

- Download the zip file for both mentioned Github repositories in the Reference section
- Unzip the zip file
- In `darknet/cfg` and `yolov4_darknet/cfg` you can find the cfg files which you can copy to the cfg folder if not already existing 
- In `darknet/data` and `yolov4_darknet/data` you can find the `.names` (list of classes) files, e.g. `coco.names` 