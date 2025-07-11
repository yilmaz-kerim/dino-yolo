# dino-yolo
The dataset includes 686 images.
Objects are annotated in YOLO v5 PyTorch format.

The following pre-processing was applied to each image:
* Auto-orientation of pixel data (with EXIF-orientation stripping)
* Resize to 640x640 (Fit (white edges))

The following augmentation was applied to create 3 versions of each source image:
* Randomly crop between 0 and 20 percent of the image

```
📦 
├─ data
│  ├─ images
│  │  ├─ test
│  │  ├─ train
│  │  └─ valid
│  └─ labels
│     ├─ test-labels
│     ├─ train-labels
│     └─ valid-label
└─ data.yaml
```

