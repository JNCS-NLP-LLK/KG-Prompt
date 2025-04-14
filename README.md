# Knowledge-guided prompt-based continual learning: Aligning task-prompts through contrastive hard negatives 
![architecture](https://github.com/JNCS-NLP-LLK/-/blob/main/KG-Prompt.png)

This repository contains official PyTorch implementation code for Knowledge-guided prompt-based continual learning: Aligning task-prompts
through contrastive hard negatives <a href="https://arxiv.org/pdf/2112.08654.pdf">KG-Prompt</a>.



## Installation
First, clone the repository locally:
```
git clone https://github.com/JNCS-NLP-LLK/KG-Prompt
cd KG-Prompt
```
Then, create a conda environment with pytorch and scikit-learn
```
conda create --name my_env python=3.8
conda activate my_env
pip install -r requirements.txt
```

## Data preparation
If you already have CIFAR-100 or ImageNet-R, pass your dataset path to  `--data-path`.

The datasets aren't ready, change the download argument in `datasets.py` as follows

**CIFAR-100**
```
datasets.CIFAR100(download=True)
```

**ImageNet-R**
```
Imagenet_R(download=True)
```

## Training

Example Template

```
sh run.sh
```

## Evaluation
To evaluate a trained model:
```
python main.py <cifar100_lgcl or imr_lgcl> --eval
```

## Acknowledgement
We refer to the code of LGCL. Thanks for their great contributions!

## Cite

```
@article{lu2025knowledge,
  title={Knowledge-guided prompt-based continual learning: Aligning task-prompts through contrastive hard negatives},
  author={Lu, Heng-yang and Lin, Long-kang and Fan, Chenyou and Wang, Chongjun and Fang, Wei and Wu, Xiao-jun},
  journal={Knowledge-Based Systems},
  pages={113009},
  year={2025},
  publisher={Elsevier}
}
```

