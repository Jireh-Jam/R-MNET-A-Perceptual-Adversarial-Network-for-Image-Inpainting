![](https://img.shields.io/badge/Python-3.6-yewllo.svg) ![](https://img.shields.io/badge/Keras-2.3.1-yewllo.svg) ![](https://img.shields.io/badge/TensorFlow-1.13.1-yewllo.svg) ![](https://img.shields.io/badge/License-MIT-yewllo.svg)
# R-MNET-A-Perceptual-Adversarial-Network-for-Image-Inpainting in Keras
R-MNET: A Perceptual Adversarial Network for Image Inpainting. 
Jireh Jam, Connah Kendrick, Vincent Drouard, Kevin Walker, Gee-Sern Hsu, Moi Hoon Yap
###
Keras implementation of R-MNET model proposed at WACV2021.
###
https://arxiv.org/pdf/2008.04621.pdf


### Architecture
<img src="https://user-images.githubusercontent.com/16281283/98450574-a29b4480-2135-11eb-871f-fe14c823e275.png" width="1000">

## Requirements
### Images dataset
[Download Places2 Dataset]( http://data.csail.mit.edu/places/places365/places365standard_easyformat.tar) and [CelebA-HQ Dataset](https://github.com/willylulu/celeba-hq-modified)
### Mask dataset
The training mask dataset used for training our model: [QD-IMD: Quick Draw Irregular Mask Dataset](https://github.com/karfly/qd-imd)   
The NVIDIA's mask dataset is available [here](https://nv-adlr.github.io/publication/partialconv-inpainting)
- Python 3.6
- Tensorflow 1.13.1
- keras 2.3.1
- opencv
- Numpy

### Training and Testing scripts.
Use the run.py file to train the model and test.py to test the model. We recommend training for 100 epochs as a benchmark based on the state-of-the-art used to compare with out model.
## Code Reference
1. Wasserstain GAN was implemented based on: [Wasserstein GAN Keras](https://github.com/eriklindernoren/Keras-GAN/blob/master/wgan/wgan.py)
2. Generative Multi-column Convolutional Neural Networks inpainting model in Keras : [Image Inpainting via Generative Multi-column Convolutional Neural Networks](https://github.com/tlatkowski/inpainting-gmcnn-keras/)
3. Nvidia Mask Dataset, based on the paper: [Image Inpainting for Irregular Holes Using Partial Convolutions](https://eccv2018.org/openaccess/content_ECCV_2018/papers/Guilin_Liu_Image_Inpainting_for_ECCV_2018_paper.pdf)
## Citing this script
If you use this script, please consider citing [R-MNet](https://arxiv.org/abs/2008.04621):
```
@inproceedings{jam2021r,
  title={R-mnet: A perceptual adversarial network for image inpainting},
  author={Jam, Jireh and Kendrick, Connah and Drouard, Vincent and Walker, Kevin and Hsu, Gee-Sern and Yap, Moi Hoon},
  booktitle={Proceedings of the IEEE/CVF Winter Conference on Applications of Computer Vision},
  pages={2714--2723},
  year={2021}
}
```
```
@article{jam2020r,
  title={R-MNet: A Perceptual Adversarial Network for Image Inpainting},
  author={Jam, Jireh and Kendrick, Connah and Drouard, Vincent and Walker, Kevin and Hsu, Gee-Sern and Yap, Moi Hoon},
  journal={arXiv preprint arXiv:2008.04621},
  year={2020}
}
```


