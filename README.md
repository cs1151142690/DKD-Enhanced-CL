

## Requirements

- Python 3
- CUDA 11
- yaml
- PIL
- tqdm
- PyTorch=1.7.1
- torchvision



## Dataset

All the used dataset are publicly-accessible:

[EyePACS](https://www.kaggle.com/c/diabetic-retinopathy-detection/data)

[IDRiD](https://idrid.grand-challenge.org/)

[Messidor](https://www.adcis.net/en/third-party/messidor/)



## Running

Stage1: Construct of positive patch set and negative patch set

Stage2: Train the teacher model

```
$ python train.py
```

Stage3: Train the student model

```
$ python student_train.py
```



## Acknowledgment

Thanks for the [Lesion_CL]([GitHub - YijinHuang/Lesion-based-Contrastive-Learning: This is the official implementation of the paper Lesion-based Contrastive Learning for Diabetic Retinopathy Grading from Fundus Images.](https://github.com/YijinHuang/Lesion-based-Contrastive-Learning)) for the lesion detection network and the implementation of models, [MoCo](https://github.com/facebookresearch/moco) for the contrastive loss. 