# GOV-NeSF

This is the official repository of the CVPR 2024 paper **"GOV-NeSF: Generalizable Open-Vocabulary Neural Semantic Fields"**. 

## Installation

To get started, follow the [Installation from NeRF-Det](https://github.com/facebookresearch/NeRF-Det) and install ```requirements.txt```.


## Acquiring Datasets


## Running the Code

### Training

Train the model as:

```bash
bash tools/dist_train.sh configs/gov_nesf/train/train.py [NUM_GPUS] [WORK_DIR]
```

For example:
```bash
bash tools/dist_train.sh configs/gov_nesf/train/train.py 1 work_dirs/train
```

### Evaluation

To evaluate the 2D segmentation, run:

```bash
bash tools/dist_train.sh configs/gov_nesf/test/scannet_test2d.py [NUM_GPUS] [WORK_DIR] [CHECKPOINT_PATH]
```

And for 3D segmentation, run:
```bash
bash tools/dist_train.sh configs/gov_nesf/test/scannet_test3d.py [NUM_GPUS] [WORK_DIR] [CHECKPOINT_PATH]
```


## BibTeX

```
@inproceedings{wang2024gov,
  title={GOV-NeSF: Generalizable Open-Vocabulary Neural Semantic Fields},
  author={Wang, Yunsong and Chen, Hanlin and Lee, Gim Hee},
  booktitle={Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition},
  pages={20443--20453},
  year={2024}
}
```

## Acknowledgements

This work is supported by the Agency for Science, Technol- ogy and Research (A*STAR) under its MTC Programmatic Funds (Grant No. M23L7b0021).
