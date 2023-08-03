---
layout: page
title: Python
subtitle: 12.Advance
menubarcount: 2
menubar: study
menubar2: study_python_menu
show_sidebar: false
hero_image: /path/to/title.jpg
hero_darken: true
toc: true
toc_title: 목차
description: 
---

## **삼항연산자**
단순 True or False 인 상황에서 가독성을 높이는데 좋음
```
if <state1>:
    <case1>
else:
    <case2>
----------------
<case1> if <state1> else <case2>
```
$ _ {23.08.03}$<br/><br/>

## **리스트 컴프리헨션(list comprehension)**
리스트를 만드는데 있어서 효과적으로 제작하는방법
```
list1 = []
for i in range(1, 11):
    list1.append(i)
----------------
list1 = [i for i in range(1, 11)]
```
$ _ {23.08.03}$<br/><br/>

## **삼항연산자 & 리스트 컴프리헨션**

```
<list> = [<data> for <data> in <datas> if <state>]

```
$ _ {23.08.03}$<br/><br/>

## **딕셔너리형 합치기**

```
<dic1> = {'am': 10}
<dic2> = {"a": 20, "b": 50}
<dic1>.update(<dic2>)
----------------
<dic1> = {'am': 10}
<dic2> = {"a": 20, "b": 50}
<dic3> = {**<dic1>, **<dic2>}
```
$ _ {23.08.03}$<br/><br/>




{% include tag.html tag="python" %}  {% include tag.html tag="Advanced skill" %}