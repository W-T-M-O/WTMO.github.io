---
layout: page
title: DL
subtitle: 5.advance
menubarcount: 2
menubar: study
menubar2: study_dl_menu
show_sidebar: false
hero_image: /path/to/title.jpg
hero_darken: true
toc: true
toc_title: 목차
---

## grid search
여러개의 파라미터를 한번에 활용해서 결과를 도출

```
from sklearn.model_selection import GridSearchCV

params = {
    <parameter>: [],
    <parameter>: [],
}
model = <imported_model>()
models = GridSearchCV(model, params, cv = 5)
models.fit()
models.best_params_
```
> * cv: cross validation

## feature importance(random forest)
어떤 feature가 결과에 영향을 크게 미쳤는지 확인하는 방법
```
data = model.feature_importances_
```

$ _ {23.08.11}$<br/><br/>



{% include tag.html tag="DL" %}  {% include tag.html tag="advance" %}