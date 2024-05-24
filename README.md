# TTA 간단 실험
- AdaBN
- TENT
- [CoTTA](https://arxiv.org/abs/2203.13591)

2024-1. 사회문제해결을위한ICT드론기술 수업 과제

  
평가 데이터
+ CIFAR100 -> CIFAR100-C (Classification)

## 사전 준비
아래 명령어를 실행해서 환경 세팅 수행
```bash
# It may take several minutes for conda to solve the environment
conda update conda
conda env create -f environment.yml
conda activate cotta 
```

## Classification 실험
### CIFAR100-to-CIFAR100C task
```bash
# Tested on A6000
bash run_cifar100.sh
```
- 위 코드를 수행하면 Source, AdaBN, TENT, CoTTA 에 대한 TTA 수행 결과가 모두 나옴!
