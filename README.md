# Score-balanced Loss for Multi-aspect Pronunciation Assessment

This repository is the implementation of the paper, [**Score-balanced Loss for Multi-aspect Pronunciation Assessment**](https://www.isca-speech.org/archive/interspeech_2023/do23b_interspeech.html) (Interspeech 2023).

> Our code is based on the open source, [https://github.com/YuanGongND/gopt](https://github.com/YuanGongND/gopt) (Gong et al, 2022).

## Dataset

An open source dataset, SpeechOcean762 (licenced with CC BY 4.0) is used. You can download it from [https://www.openslr.org/101](https://www.openslr.org/101).

## Package Requirements

Install below packages in your virtual environment before running the code.
- python version 3.8.10
- pytorch version '1.13.1+cu117'
- numpy version 1.20.3
- pandas version 1.5.0

You can run below command on your virtual environment
- `pip install -r requirements.txt`

## Training and Evaluation (GOPT with SB Loss)
This bash script will run each model 5 times with ([0, 1, 2, 3, 4]).
- `cd src`
- `bash run_SB_pred.sh`

Note that every run does not produce the same results due to the random elements.

## Run baseline (GOPT)
This bash script will run each model 5 times with ([0, 1, 2, 3, 4]).
- `cd src`
- `bash run_gopt.sh`

## Citation
Please cite our paper, if you find this repository helpful.

```@inproceedings{do23b_interspeech,
  author={Heejin Do and Yunsu Kim and Gary Geunbae Lee},
  title={{Score-balanced Loss for Multi-aspect Pronunciation Assessment}},
  year=2023,
  booktitle={Proc. INTERSPEECH 2023},
  pages={4998--5002},
  doi={10.21437/Interspeech.2023-1679}
}```