# 2022Hanium_AdvDef
---
과학기술정보통신부 정보통신창의인재양성사업의 지원을 통해 수행한 2022 ICT멘토링 프로젝트 결과물로, 적대적 AI 공격에 대한 인공지능 보안기술 구현 프로젝트입니다.


### 프로젝트 설명
---
자율주행의 시대가 도래함에 따라 딥러닝 , 모델에 대한 적대적 공격 위험이 함께 증가하고 있습니다. 카메라 기반 자율주행차량이 공격받을 경우 보행자나 표지판 등에 대한 오분류로 인해 심각한 사고로이어질 수 있어 자율주행 , 시스템에서의 적대적 공격에 대한 방어 및 보안 기술 연구가 필수적입니다. 이에 본 연구에서는 GTSRB 표지판 데이터를 이용하여 각종 공격 및 방어 기법을 개발하고 제안합니다. 시간 및 정확도 측면에서 성능을 비교함으로써 자율주행에 , 최적인 모델을 탐구하고 더 나아가 해당 모델들의 완전자율주행을 위한 발전 방향을 제안합니다.

### 데이터셋
---
GTRSB 데이터셋

### 기술스택 
---
PYTHON

### 개발 내용 
---
#### 분류 모델
```
python .py \
  --data_name 'data_test' \
  --model_name 'model' \
  --epoch 30\
  --overwrite_output_dir True
  
```

#### 방어모델
- MagNet
```
python 21011_MagNet_FGSM.ipynb\
  --data_name 'data_test' \
  --model_name 'fgsm_attack' \
  --epoch 100\
  --overwrite_output_dir True
```

#### 공격모델
- FGSM
```
python 220709_FGSM_CNN.ipynb \
  -- data_name 'data_test' \
  -- model_name 'fgsm_attack' \
  --step_size 2 (alpha 값) \
  --num_steps 7 (iterations 값) \
  -- eps 0.02, 0.03, 8/255, 0.05, 0.08, 0.10\
  -- overwrite_output_dri True
```  



### 수행결과
---
- 2022 한이음 ICT멘토링 프로젝트 (22_HF383)
- ACK 2022 학술발표대회 논문집 **논문 게재** (제29권 제2호 p.803 - p.805)
    - 온라인 논문집 : [http://kips.or.kr/bbs/confn/article/2484](http://kips.or.kr/bbs/confn/article/2484)
    - 발표 영상 : [https://youtu.be/7-XDBGTxpEU](https://youtu.be/7-XDBGTxpEU)
- 2022 한국정보처리학회 ICT멘토링 학술대회 (ACK 2022) **최우수상**
- 2022 한이음 공모전 **입선**
    - 영상링크 : [https://youtu.be/WCH_ouw3U8A](https://youtu.be/WCH_ouw3U8A)
