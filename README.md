# <div align="center">FCRN: Fast contamination recognition network</div>

<div align="center"><b>Fast contamination recognition network: a knowledge distillation based hyperspectral outdoor insulator contamination level recognition network</b></div>

<div align="center">Junbo Zhou, Guoqiang Gao*, Yujun Guo, Pu Zhang, Kangle Wang, Xueqin Zhang, Song Xiao, Guangning Wu</div>

<div align="center">Southwest Jiaotong University, *Corresponding author</div><br>

<div align="center"><img alt="Static Badge" src="https://img.shields.io/badge/FCRN-paper-blue?link=https%3A%2F%2Fwww.sciencedirect.com%2Fscience%2Farticle%2Fpii%2FS0957417425040163"></div>

## Overview
**FCRN** is a novel knowledge distillation based hyperspectral outdoor insulator contamination level recognition network. It effectively integrates state-of-the-art knowledge distillation methods to fulfill the growing demand for lightweight yet powerful insulator contamination level recognition models.
![Structure](https://github.com/IIMARSS/FCRN/blob/main/Overall%20structure.png?raw=true)

## How to start
### *Installation*
**Step 1: Cloning the repository**<br>
```
git clone https://github.com/IIMARSS/FCRN.git
```
**Step 2: Environment setup**<br>
Following the requirements and installing the packages.
```
pip install -r requirements.txt
```
### *Data preparation*
Download the insulator contamination HSI datasets from [Google Drive](https://drive.google.com/file/d/1u48ZmYHVyNuiqHAcVywEm-Bh1HghumuL/view?usp=drive_link) or [Baidu Drive](https://pan.baidu.com/s/1sWUwkPWzrYLBcNUqadY09Q?pwd=2333) and put them under the [Datasets] folder. Of course, you can use the public HSI datasets or your own datasets as well. It will have the following structure:
```
${DATASET_ROOT}   # Dataset root directory
├── Datasets
│   │
│   ├── xianchang1        # Sunny condition
│   │   ├──xianchang1_2.mat
│   │   ├──xianchang1_2_gt.mat
│   │
│   ├── xianchang2  # Cloudy condition
│   │   ├──xianchang2.mat
│   │   ├──xianchang2_gt.mat
│   │
│   ├── ip         # Indian Pines data	
│   │   ├──Indian_pines_corrected.mat
│   │   ├──Indian_pines_gt.mat 
│   │
│   ├── other HSI Datasets   
│   │   ├ ... 
│   │    

```
### *Running the code*
```
python main.py --model kd --dataset xianchang1
```
## Reference
If you find our model is useful for your research, please cite our paper! We are very grateful for your support!❤️❤️
```
@article{zhou2025fast,
  title={Fast contamination recognition network: a knowledge distillation based hyperspectral outdoor insulator contamination level recognition network},
  author={Zhou, Junbo and Gao, Guoqiang and Guo, Yujun and Zhang, Pu and Wang, Kangle and Zhang, Xueqin and Xiao, Song and Wu, Guangning},
  journal={Expert Systems with Applications},
  pages={130401},
  year={2025},
  publisher={Elsevier}
}
```
## Questions
If you have any questions, [please let me know](imjbzhou@my.swjtu.edu.cn)!<br>
## Thanks
Our project is based on [DeepHyperX](https://github.com/eecn/Hyperspectral-Classification). Thanks for the wonderful work.🌹🌹
