# SwUniv_Capstone Project
### 2021년 SW융합캡스톤디자인 프로젝트 최종결과
##### (복사본)
-----------------------------------------------------------------------------------
## 유전자 발현 데이터 기반의 항암제 약물 반응성 예측을 위한 딥러닝/머신러닝 모델 연구

### 프로젝트 일정
- 4/29 중간발표
- 6/17 기말발표

#### Team Member
- 곽도현
- 마희선
- 한수호

#### Feedback
##### 1. 중간발표 피드백
* label encoding -> one-hot encoding
* feature selection 고려

##### 2. 21.05.21 피드백

* Dataset 조정
  - 대장암 특정
    - 3개 정도의 암으로 확장 (암끼리 특성이 비슷해서 모델에 크게 문제가 없을 수 있음)
* 약물 Label 개수 조정 (상위 6개 -> 3개)

* Feature selection 
  - Dimension reduction(PCA) 먼저 해보고 이후에 feature selection 고려
  - Feature selection 시에 biolgical 개념 추가

* Model
  - Keras sequential
  - ML Model (SVM, RF 등의 모델 추가)
    - Confidence interval 기반의 Train set subsampling 해서 모델 학습
    - Cross validation

* Evaluation
  - Accuracy 외에 AUC 같은 평가척도도 활용
    - Multi label data인 경우에 macro/micro AUC를 사용해서 평가하는 것이 더 신뢰성 높음


