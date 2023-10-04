# Face_Mask_Detection

## Dataset
The Dataset used in this project is available in Kaggle and can be downloaded from [here](https://www.kaggle.com/datasets/andrewmvd/face-mask-detection). <br>
It consists of images and corresponding labels for three different classes as follows: <br>
  1. With Mask ["WM"]
  2. Without Mask ["WoM"]
  3. Mask wore incorrect ["MWI"]

## Preprocessing
The given labels are in Pascal VOC format (XML) they should be converted into YOLO format (Text) for training. After that data is split into 80:20 ratio.

## Training
The model is trained using the given dataset for ~120 epochs. Other parameters are <br>
Image size : 640 x 640 <br>
Batch size : 32

## Metrics
Class/Metric | Precision | Recall |  mAP50  | mAP50-95| F1 Score |Accuracy
------|-----------|--------|---------|---------|----------|---------
All   |  0.816    | 0.764  |  0.831  | 0.560   | 0.7891   | 92.45%
WM    |  0.944    | 0.908  |  0.956  | 0.655   | 0.9256   | 88.06%
WOM   |  0.787    | 0.752  |  0.790  | 0.475   | 0.691    | 91.39%
MWI   |  0.717    | 0.633  |  0.747  | 0.551   | 0.6723   | 97.84%

## Results

