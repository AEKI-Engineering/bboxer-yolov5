# bboxer-yolov5

AEKI Engineering YOLOv5 (release v6.2) bounding boxer training code.

# Table of contents

1. [Prerequisities](#prerequisities)
2. [Datasets](#datasets)
3. [Appendix](#appendix)

# Prerequisities

Install dependencies from lock file with **Poetry**:

```sh
poetry install --no-root
poetry shell
```

For more information about Poetry, visit [this handy document](https://www.notion.so/Poetry-101-eaf98d54e5974765801f5ac48b164196).

# Datasets

Dataset definitions are stored inside `data` directory and contain `aeki` prefix:

```sh
.
├── data
│   ├── aeki-coco.yaml
│   ├── aeki-coco128.yaml
│   └── [...]
└── [...]
```

Data is stored inside `dataset` directory, under path defined in `yaml` dataset definiton:

```yaml
# Contents of data/aeki-yolo.yaml file
path: ./datasets/coco # dataset root dir
train: images/train # train images (relative to 'path')
val: images/val # val images (relative to 'path')
test: # test images (optional)
```

For more information about datasets and classes, visit [dataset index](https://www.notion.so/Datasets-index-03976afb21c54acd96cc5bf867287e6d).

# Appendix

## Project status

Created 31-08-2022. Forked from [YOLOv5 repository](https://github.com/ultralytics/yolov5/tree/55b009616b4701f73311d1272cc87057d84a93e6), latest commit ID: 55b0096