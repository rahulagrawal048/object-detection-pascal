# object-detection-pascal
Pytorch implementation of FCOS and Faster-RCNN for object detection on PASCAL dataset

I implement a one-stage object detector based on [FCOS: Fully-Convolutional One-Stage Object Detection](https://arxiv.org/abs/1904.01355) and train it to detect a set of object classes. Our detector design is highly similar to FCOS itself, except we train a smaller model with slightly different hyperparameters to manage with limited resources on Colab.
I also evaluate the detection accuracy using the classic metric mean Average Precision (mAP).

For FCOS, mAP = 43.25%

Next, I implement a two-stage object detector, based on [Faster R-CNN](https://arxiv.org/pdf/1506.01497.pdf), which consists of two modules - Region Proposal Networks (RPN) and Fast R-CNN. Like one-stage detector in the first part, I train it to detect a set of object classes and evaluate the detection accuracy using the classic metric mean Average Precision (mAP).

For Faster-RCNN, mAP = 45.22%
