# YOLOv3-Face_Training
In this repo, you can see training and validation files with an appropriate darknet

## Arranging Darknet
After clonening the repo, you must write command line to make. If your GPU has different architecture you must set it. Also you must arrange cuda and nvcc directories for using GPU=1. After arranging this files, you must write to command line make. If there is no error, you can start training.

## Starting Training
All the configuration files and training images prepared. If you want to start training, you must only write the command below.
```
./darknet detector train cfg/face.data cfg/face.cfg yolov3.conv.81 -map
```

 If you don't have pre-trained model you can prepare it with using this command. If you don't have [yolov3.weights](https://pjreddie.com/media/files/yolov3.weights) you can download it by clicking.

```
./darknet partial cfg/yolov3.cfg yolov3.weights yolov3.conv.81 81
```
