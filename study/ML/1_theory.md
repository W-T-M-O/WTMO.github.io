---
layout: page
title: ML
subtitle: 1.theory
menubarcount: 2
menubar: study
menubar2: study_ml_menu
show_sidebar: false
hero_image: /path/to/title.jpg
hero_darken: true
toc: true
toc_title: 목차
---

## Linear Regression
종속변수와 독립변수간에 관계를 예측하는 모델로 선형적 모델을 가지고 종속변수와 독립변수의 관계를 도출하는 방법이다.
## Logistic Regression
종속변수와 독립변수간에 관계를 예측하는 모델로 linear regression과 다르게 이항, 다항과 같이 항을 기준으로 classification을 한다.
* odds  
성공확률과 실패 확률의 비율  

$$odds = \tfrac{p(y=1|x)}{1-p(y=1|x)}$$

* logit  
odds에 log를 취한 함수  

$$logit(p) = log(\tfrac{p}{1-p})$$

* logistic function  
logit을 기반으로 만든 함수로 0에서 1까지 곡선형을 가진다.  

$$logistic \, function = \tfrac{e^{\beta X_i}}{1+e^{\beta X_i}}$$

## Decision Tree
Tree 구조로 형성된 의사결정 분류 알고리즘
## Naive Bayes
특성들 사이의 독립을 가정하는 베이즈 정리를 이용한 확률 분류기
* Bayes Theorem  
어떠한 기존의 확률을 토대로 새로운 데이터의 확률을 구하는 방법

$$P(c\|x)=\tfrac{P(x\|c)P(c)}{P(x)}$$
* elements
    * $P(c\|x)$ posterior probabillity

    * $P(x)$ predictor prior probabillity  
    어떠한 기존의 발생 확률

    * $P(c)$ class prior probabillity  
    어떠한 특성을 가질 확률

    * $P(x\|c)$ likelihood
    특성에서의 발생이 될 확률

## Support Vector Machine(SVM)
카테고리들이 있을때 데이터들의 사상된 공간의 경계중 가장 큰 너비를 가진 경계를 찾는 방법
* margin  
서로 다른 두가지 클래스의 데이터에서 어떠한 선으로 구분을 할경우 해당 선의 너비를 의미한다.
* support vectors  
margin에 해당하는 위치에 놓여있는 elements를 의미한다.
* RBF(Radial Basis Fuction) Kernel
방사형 기저 함수라 불리며 차원을 높여서 margin을 설계하는 방법

## K Nearest Neighbors(KNN)
새로운 데이터를 입력받을때 가까운 데이터들의 분포에 따라 통계적으로 분류를 하는 알고리즘
## Bagging VS Boosting
* bagging  
분산을 감소시키는 방법으로  
복원 추출을 통해 n개의 샘플을 만드는 boostraping을 통해 나온 샘플을 학습시켜서 선형 결합한것

* boosting  
편항을 감소시키는 방법으로  
weak learner를 생성해서 구한 error를 토대로 가중치를 가해 error를 줄이는 방법이다.

## Decision Tree ensemble
* ensemble  
우수한 모델들에서 나온 결과를 선형적으로 결합하여 성능을 향상하는 방법
### Random Forest
bagging을 사용한 알고리즘으로 모든 변수를 기반으로 Tree 생성
### Extra Trees Boosting
boosting을 사용한 알고리즘으로 무작위 변수로 weak tree를 생성하여 진행
## Decision Tree Gradient Boosting
* Gradient Boosting은 미분을 통해 Residual을 줄이는 방향으로 weak learner들을 결합하는 방법(과적합 이슈의 발생)
### Extreme Gradient Boosting(XGB)
Regularization과 다양한 loss function을 지원하여 과적합을 감소시킨 방법
### Light Gradient Boosting
histogram-based/GOSS/EFB와 같은 알고리즘으로 학습데이터를 감소시켜 속도를 향상시킨 방법(데이터가 적으면 과적합 위험)
### Categorical Gradient Boosting
범주형 변수를 위한 알고리즘으로 one-hot encoding사용시 증폭되는 메모리 이슈를 보완하였음
### Natural Gradient Boosting
각 예측값에 대한 신뢰도를 도출해주는 알고리즘으로 시간이 오래걸리는 단점이 있음

$ _ {23.08.21}$<br/><br/>



{% include tag.html tag="ML" %}  {% include tag.html tag="theory" %}