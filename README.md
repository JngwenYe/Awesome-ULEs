# Awesome Unlearnable Examples

[![Awesome](https://awesome.re/badge.svg)](https://awesome.re)
<!--[![arXiv](https://img.shields.io/badge/arXiv-2209.02299-b31b1b.svg)](https://arxiv.org/abs/2209.02299)
[![Static Badge](https://img.shields.io/badge/Kaggle-Notebook-4388f7)](https://www.kaggle.com/code/tamlhp/machine-unlearning-the-right-to-be-forgotten/)
[![Website](https://img.shields.io/website?down_color=lightgrey&down_message=offline&label=Official%20Website&up_color=green&up_message=online&url=https%3A%2F%2Fawesome-machine-unlearning.github.io%2F)](https://awesome-machine-unlearning.github.io/)
![GitHub stars](https://img.shields.io/github/stars/tamlhp/awesome-machine-unlearning?color=yellow&label=Stars)
[![Hits](https://hits.seeyoufarm.com/api/count/incr/badge.svg?url=https%3A%2F%2Fgithub.com%2Ftamlhp%2Fawesome-machine-unlearning&count_bg=%2379C83D&title_bg=%23555555&icon=&icon_color=%23E7E7E7&title=hits&edge_flat=false)](https://hits.seeyoufarm.com)-->

<img src="https://img.shields.io/badge/Contributions-Welcome-278ea5" alt="Contrib"/>

A collection of academic articles, published methodology, and datasets on the subject of **unlearnable examples**.




## Unlearnable Examples
![ULEs](figs/unlearn.png) Unlearnable examples (ULEs) refer to data points or scenarios that are exceptionally challenging or even impossible for machine learning models to learn or generalize from due to factors such as noisy data, lack of information, complexity, conceptual limitations, adversarial input, or insufficient data, posing significant challenges to the capabilities of the models. Researchers continuously strive to overcome these limitations through algorithmic improvements and data enhancements..


## Common Experimental Settings
- Dataset: [CIFAR-10](https://www.cs.toronto.edu/~kriz/cifar.html), [CIFAR-100](https://www.cs.toronto.edu/~kriz/cifar.html), [ImageNet-100](https://www.kaggle.com/datasets/ambityga/imagenet100), [Tiny-ImageNet](https://www.kaggle.com/competitions/tiny-imagenet/overview), ...
- Architectures: ResNet-18, VGG-16, Wide ResNet-34-10, DenseNet-121,...
- Perturbations: $\|\delta\|_{\infty}\le \epsilon$, where $\epsilon = \{ 4/255,8/255\}$; $\|\delta\|_{2}\le \epsilon$, where $\epsilon = \{ 0.25,0.5,0.75\}$,...

## Evaluations
### The goal is to generate noise in order to protect the personal images with two requirements:
1. The generated noise must be non-suspicious.
2. When training a model on the perturbed images, the model must not be able to learn to predict the classes corresponding to clean images. 


### Tasks: 
  
### Evaluation Metrics:
  
<br>
<br>




## Published Papers
<br>

### Generating ULEs
| **Paper Title** | **Year** | **Author** | **Venue** | **Method** | **Code** |
| --------------- | :----: | ---- | :----: | :----: | :----: | 
|[Unlearnable Clusters: Towards Label-Agnostic Unlearnable Examples](https://arxiv.org/abs/2301.01217)|2023|Zhang et al. |CVPR| Unlearnable Clusters |[[Code]](https://github.com/jiamingzhang94/Unlearnable-Clusters) |
|[CUDA: Convolution-based Unlearnable Datasets](https://arxiv.org/abs/2303.04278)|2023|Sadasivan et al. | CVPR | Convolutional Filters |[[Code]](https://github.com/vinusankars/Convolution-based-Unlearnability)
| [Transferable Unlearnable Examples](https://arxiv.org/abs/2210.10114) | 2023 | Ren et al. | ICLR | Data-wise and Training-wise Transferability  | - |
| [Robust unlearnable examples: Protecting data against adversarial learning](https://arxiv.org/abs/2203.14533)|2022| Fu et al.|ICLR| Robust error-minimizing noise | [[Code]](https://github.com/fshp971/robust-unlearnable-examples})|2023|
| [Unlearnable Examples: Making Personal Data Unexploitable](https://arxiv.org/abs/2309.00886) | 2021 | Huang et al. | ICLR | Error-minimizing Noise| [[Code]](https://github.com/HanxunH/Unlearnable-Examples) | 
|[Going Grayscale: The Road to Understanding and Improving Unlearnable Examples](https://arxiv.org/abs/2111.13244)| 2021| Liu et al.|Arxiv|ULEO-GrayAugs|[[Code]](https://github.com/liuzrcc/ULE-GrayAug) |
----------
<br>

### Against ULEs
| **Paper Title** | **Year** | **Author** | **Venue** | **Method** | **Code** |
| --------------- | :----: | ---- | :----: | :----: | :----: | 
|[Unlearnable Examples Give a False Sense of Security: Piercing through Unexploitable Data with Learnable Examples](https://arxiv.org/abs/2305.09241)|2023|Jiang et al.|MM||[[Code]](https://github.com/jiangw-0/LE_JCDP)|
|[Image Shortcut Squeezing: Countering Perturbative Availability Poisons with Compression.](https://arxiv.org/abs/2301.13838)|2023| Liu et al.|ICML| Compression-based Method | [[Code]](https://github.com/liuzrcc/ImageShortcutSqueezing)|
[Learning the Unlearnable: Adversarial Augmentations Suppress Unlearnable Example Attacks](https://arxiv.org/abs/2303.15127)|2023|Qin et al.|Arxiv | Adversarial augmentations|[[Code]](https://github.com/lafeat/ueraser)|
[The Devil's Advocate: Shattering the Illusion of Unexploitable Data using Diffusion Models](https://arxiv.org/abs/2303.08500)|2023|
------