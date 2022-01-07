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
* feature를 만들 수 있는 모든 경우의 수를 고려해서 만들었다.
* feature selection 하기 전의 데이터셋 용량이 2기가 정도 되었다.
* 36000개 정도 만들었었는데, 이때 차원의 저주를 직접 체험하게 되었다.
* feature selection에 있어서 많은 고민을 했던 대회였다.
* 대회를 진행함에 있어서 끝까지 최선을 다할 수 있는 체력이 중요한 요소임을 깨달았다.
* 두 명이 팀플로 진행했는데 팀메이트의 중요성 또한 깨닫게 되었다.
## LB
* (public) 8.07147 : 5th / 18
* (private) 7.99473 : 5th / 18
