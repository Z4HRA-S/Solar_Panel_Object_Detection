# Solar_Panel_Object_Detection
# README

This Project aims to use Unet, MaskedRCNN, PSP, and FPN to segment and detect solar panels in satellite photos. 

## DataSet

The link to the data set: [Link](https://zenodo.org/record/5171712)

## 1. Directory Tree

```
│  
└───test_panel_data   # random test images from the net
│  
└───EDA_and_data_preprocessing.ipynb # a notebook containing data exploration and data preprocessing
│  
└───segmentation_train.ipynb  # contain the process of training an Unet for segmentation
│  
└───PSP_semantic_segmentation_train.ipynb  # contain the process of training a PSP net for segmentation
│  
└───FPN_segmentation_train.ipynb  # contain the process of training a FPN net for segmentation
│  
└───object_detection_train.ipynb # contain the process of finetuning a MaskedRCNN for segmentation
│  
└───Evaluation.ipynb # evaluating the saved model from above notebooks

```


## Run

:::warning
run `%cd` command based on your own directory path.
:::

For this code,
you need to place these files from [this repo](https://github.com/pytorch/vision/tree/main/references/detection) in the root project directory:
- utils.py
- transforms.py
- engine.py
- coco_utils.py
- coco_eval.py

The order of running the notebooks is as follows. However, because the result of every step is saved you can run codes from any step you want.

1. EDA_and_data_preprocessing.ipynb
2. segmentation & object detection
3. Evaluation.ipynb

