---
layout: page
title: ML
subtitle: 1.
menubarcount: 2
menubar: study
menubar2: study_ml_menu
show_sidebar: false
hero_image: /path/to/title.jpg
hero_darken: true
toc: true
toc_title: 목차
---

## LinearRegression
선형적인 모델로 예측이 될때 사용
```
from sklearn.linear_model import LinearRegression
```

## LogisticRegression
0과1 처럼 나뉘어지는 형태 또는 0~1로 나뉘어지는 모델
```
from sklearn.linear_model import LogisticRegression
```

## DecisionTreeRegressor
tree 형태로 구분이 되며 feature들에 따라 결과를 다각형의 직선으로 표현하는 형태이다

```
from sklearn.tree import DecisionTreeRegressor

model = DecisionTreeRegressor(random_state=100, min_samples_leaf=1, min_samples_split=5, max_depth=5)
```
> * random_state 시드값
> * max_depth 최대 깊이
> * min_samples_leaf 리프 원소의 최소갯수
> * min_samples_split root 원소의 최소갯수

## RandomForestClassifier
다수의 트리들을 랜덤하게 학습하는 방법으로 과적합을 방지하기 위해 탄생하였으나 비교적 느리다. feature들에 따라 결과를 구역으로 나뉘는 형태이다.

```
from sklearn.ensemble import RandomForestClassifier
```
$ _ {23.08.10}$<br/><br/>



{% include tag.html tag="ML" %}  {% include tag.html tag="model" %}