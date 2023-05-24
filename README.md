# MALUNet
This is the official code repository for "MALUNet: A Muti-Attention and Light-weight UNet for Skin Lesion Segmentation", which is accpeted by *IEEE International Conference on Bioinformatics and Biomedicine (BIBM2022)* as a regular paper! [[arxiv]](https://arxiv.org/abs/2211.01784)

**0. Main Environments**
- python 3.8
- pytorch 1.8.0
- torchvision 0.9.0

**1. Prepare the dataset.**

- The ISIC17 and ISIC18 datasets, divided into a 7:3 ratio, can be found here {[Baidu](https://pan.baidu.com/s/1Y0YupaH21yDN5uldl7IcZA?pwd=dybm) or [GoogleDrive](https://drive.google.com/file/d/1XM10fmAXndVLtXWOt5G0puYSQyI2veWy/view?usp=sharing)}. 

- After downloading the datasets, you are supposed to put them into './data/isic17/' and './data/isic18/', and the file format reference is as follows. (take the ISIC17 dataset as an example.)

- './data/isic17/'
  - train
    - images
      - .png
    - masks
      - .png
  - val
    - images
      - .png
    - masks
      - .png

**2. Train the MALUNet.**
```
cd MALUNet
```
```
python train.py
```

**3. Obtain the outputs.**
- After trianing, you could obtain the outputs in './results/'
