# dino-yolo

CURRENT: Dealing with small issues, will be updated.

This dataset was created to train a YOLO-based object detection model that could play the Chrome Dino game automatically. I started the project in early May 2025 and finished labeling the data within two weeks.

At first, I planned to train the model using YOLOv5 on my own machine with an RTX 2060 GPU. Unfortunately, the GPU stopped working the first time I tried to use it after a long break. I then considered using Google Colab for training, but I haven’t gotten around to it yet — the dataset is ready and waiting.


## General Information
The dataset includes 686 images. 
Objects are annotated in YOLO v5 PyTorch format.
All objects were labelled with Roboflow. There are 3 classes: dino, cactus and bird.

The following pre-processing was applied to each image:
* Auto-orientation of pixel data (with EXIF-orientation stripping)
* Resize to 640x640 (Fit (white edges))

The following augmentation was applied to create 3 versions of each source image:
* Randomly crop between 0 and 20 percent of the image


## Repo Structure

``` 
├─ data
│  ├─ images
│  │  ├─ test
│  │  ├─ train
│  │  └─ valid
│  └─ labels
│     ├─ test-labels
│     ├─ train-labels
│     └─ valid-labels
└─ data.yaml
```

