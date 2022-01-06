# KML Challenge 2021S
![image](https://user-images.githubusercontent.com/77089771/148399197-44b1729f-3e9d-48b5-af17-98a68533a45e.png)
## Evaluation
* RMSE(Root Mean Square Error)
## 접근방법
* 고객 ID별로 나이를 예측하는 Regression 문제
* groupby와 unstack을 통한 multi-groupby feature 생성
* 구입브랜드명 fasttext를 통한 embedding
* 구입시간, 구입물건 관련 범주형 변수 합침 -> fasttext를 통한 embedding
* sklearn의 SelectFromModel을 이용한 feature selection(threshold : 5.0 * mean)
* Bayesian Opt를 통한 하이퍼파라미터 튜닝
* LightGBM
* keras를 이용한 NN모델 앙상블
## REVIEW
* 차원의 저주를 직접 경험해 본 대회였다.
* 
## LB
* (public) 8.07147 : 5th / 18
* (private) 7.99473 : 5th / 18
