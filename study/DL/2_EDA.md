---
layout: page
title: DL
subtitle: 2.EDA
menubarcount: 2
menubar: study
menubar2: study_dl_menu
show_sidebar: false
hero_image: /path/to/title.jpg
hero_darken: true
toc: true
toc_title: 목차
---

keras.layers.Dense(10, activation="relu", kernel_initializer="he_normal")
node is 10, relu activation function, He normalize initializer

그래디언트 클래핑
optimizer = keras.optimizers.SGD(clipvalue=1.0)
optimizer = keras.optimizers.SGD(clipnorm=1.0)


# 고속 옵티마이저
* 모멘텀 최적화
경사 하강법에 모멘텀을 추가한 형태(초기에는 느린데 모멘텀을 추가로 가져서 종단속도까지 빠르게 도달함)
optimizer = keras.optimizers.SGD(learning_rate=0.001, momentum=0.9)
* 네스테로프 가속 경사  
모멘텀에 미리 한스탭 나아간것을 추가하여 진동을 감소시킴
optimizer = keras.optimizers.SGD(learning_rate=0.001, momentum=0.9, nesterov=True)


전이학습
<model>.layers[:-1] -> 최종층을 제외하고 추출
<clone_model> = keras.models.clone_model(<model>)
<clone_model>.set_weights(<model>.get_weights())


$ _ {23.08.09}$<br/><br/>



{% include tag.html tag="DL" %}  {% include tag.html tag="EDA" %}