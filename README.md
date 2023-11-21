## Barlow Twins GAN &mdash; Official PyTorch implementation

**Barlow Twins GAN: Redundancy Reduction in GAN Training with Pretrained Networks**<br>
by [Geonhui Son](https://scholar.google.co.kr/citations?user=oHpLEykAAAAJ&hl=ko&oi=ao), [Jeong Ryong Lee](https://scholar.google.co.kr/citations?user=brQgjXcAAAAJ&hl=ko&oi=ao) and [Dosik Hwang](https://scholar.google.co.kr/citations?user=PciqeBcAAAAJ&hl=ko&oi=ao). <br>

## ToDos
- [ ] Initial code release
- [ ] Providing pretrained models


## Data Preparation ##
For a quick start, you can download the few-shot datasets provided by the authors of [FastGAN](https://github.com/odegeasslbc/FastGAN-pytorch). You can download them [here](https://drive.google.com/file/d/1aAJCZbXNHyraJ6Mi13dSbe7pTyfPXha0/view). To prepare the dataset at the respective resolution, run for example
```
python dataset_tool.py --source=./data/pokemon --dest=./data/pokemon256.zip \
  --resolution=256x256 --transform=center-crop
```
You can get the datasets we used in our paper at their respective websites: 
[CLEVR](https://cs.stanford.edu/people/jcjohns/clevr/), [FFHQ](https://github.com/NVlabs/ffhq-dataset), [Cityscapes](https://www.cityscapes-dataset.com/), [LSUN](https://github.com/fyu/lsun), [AFHQ](https://github.com/clovaai/stargan-v2), [Landscape](https://www.kaggle.com/arnaud58/landscape-pictures).



## Acknowledgemnets
Our code builds upon the awesome [styleGAN2-ADA](https://github.com/NVlabs/stylegan2-ada-pytorch), [StyleGAN3](https://github.com/NVlabs/stylegan3), [ProjectedGAN](https://github.com/autonomousvision/projected-gan) and [StyleGAN-XL](https://github.com/autonomousvision/stylegan-xl/).

Furthermore, we use parts of the code of [FastGAN](https://github.com/odegeasslbc/FastGAN-pytorch), [MiDas](https://github.com/isl-org/MiDaS), [InsGen](https://github.com/genforce/insgen), [FakeCLR](https://github.com/iceli1007/FakeCLR/) and [Barlow Twins](https://github.com/facebookresearch/barlowtwins).

