# Object Detection on COCO Dataset

Object Detection is one of the fundamental tasks in computer vision with applications ranging across medicine, robotics, and many others. In this task, you are given a dataset that consists of images containing people and cars. The goal here is to train a model that can localize and classify each instance of person and car as accurately as possible.

## Dataset Details

Number of images: 2239
Size: 750 MB (approx.)
Categories: 2 (person and car)
Annotation format: COCO

Data directory structure:

  data
  
    |
    -annotations
      |
      -bbox-annotations.json
    |
    -images
      |
      -image_000000001.jpg
      |
      -image_000000002.jpg
      |
      -...
      ...
      
License: These images are taken from OpenImages. All annotations are licensed under CC BY 4.0 and the images have a CC BY 2.0 license

Link to download the dataset: https://evp-ml-data.s3.us-east-2.amazonaws.com/ml-interview/openimages-personcar/trainval.tar.gz

## Result Format

Develop and train a model on this dataset to detect person and cars in an image.

## Deliverable

1. A brief write-up about the solution explaining your assumption, approach, metrics and other artifacts.
2. A link to your solution code base, either hosted in Google Drive, OneDrive or a GitHub repository.

## Detailed Report

For a detailed explanation, follow this *[report]()*

## Approach



## Model Architecture

<img src="https://github.com/learner-subodh/EagleView_COCO-OD/blob/main/EfficientDet_Architecture.jpg?raw=true" width="1400" height="400">
EfficientDet architecture – It employs EfficientNet as the backbone network, BiFPN as the feature network, and shared class/box prediction network. Both BiFPN layers and class/box net layers are repeated multiple times based on different resource constraints

## Environment and Hardware

Google Colaboratory

Single GPU

GPU Used:

## Loss Function & Metrics

Loss Function: Focal Loss

Metric(s): Average Precision (Primary), Intersection Upon Union (Secondary)

## Results

### add images like the model arch
Refer to results folder for more such images

## Replicate Results

1. Use **EagleView_COCO-OD.ipynb**
2. Can be run either on [Google Colab](https://colab.research.google.com/notebooks/intro.ipynb) or on local environment
3. To infer an image: 
    *scripts > infer_single_image.py*

## References

1. [COCO Dataset](https://cocodataset.org/#home)
2. Google's automl repository for [efficientdet](https://github.com/google/automl/tree/master/efficientdet)
3. [EfficientDet: Scalable and Efficient Object Detection](https://arxiv.org/pdf/1911.09070.pdf)
4. Google AI Blog: [EfficientDet: Towards Scalable and Efficient Object Detection](https://ai.googleblog.com/2020/04/efficientdet-towards-scalable-and.html)
5. Analytics India Magazine: [EfficientDet: Guide to State of The Art Object Detection Model](https://analyticsindiamag.com/efficientdet/)
