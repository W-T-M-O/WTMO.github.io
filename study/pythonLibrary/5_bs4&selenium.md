---
layout: page
title: Python
subtitle: 5.bs4&selenium
menubarcount: 2
menubar: study
menubar2: study_pythonLibrary_menu
show_sidebar: false
hero_image: /path/to/title.jpg
hero_darken: true
toc: true
toc_title: 목차
---

## **requests**
python에서 가장 원형적인 파싱의 방법  
```
import requests
import json

data = requests.get("https://jsonplaceholder.typicode.com/comments")
data = json.loads(data.text)
```

## **bs4**
html과 같은 정적인 페이지에서 데이터를 분류하기 위한 라이브러리

### **import**
```
from bs4 import BeautifulSoup
```

### **request from homepage**
홈페이지에서 데이터가져오기
```
request_data = requests.get("https://naver.com")
```

### **html parsing**
가져온 데이터 html형태로 파싱하기
```
soup = BeautifulSoup(request_data.text,'html.parser')
```

### **select from parsing data**
* 파싱한 데이터에서 title 태그의 값들 가져오기
```
result = soup.select('title')[0].text
```

* tag1에 속한 자손(tag2) 가져오기
```
result = soup.select("tag1 tag2").text
```

* tag1에 속한 자식(직계 tag2) 가져오기
```
result = soup.select("tag1 > tag2").text
```

* class1 가져오기
```
result = soup.select(".class1").text
```

* id1 가져오기
```
result = soup.select("#id1").text
```

* tag1에 href 속성을 가진것 가져오기
```
result = soup.select("tag1[href]").text
```

* tag1 태그요소 중 \<num\>번째 요소 선택
```
result = soup.select("tag1:nth-child(<num>)").text
```

* 파싱한 데이터에서 title 태그의 첫번째 텍스트 가져오기
```
result = soup.select_one('title').text
```

### **header**
홈페이지에서 크롤링을 막을때 홈페이지 접근이 정상적인것 처럼할때 넣는다.  
```
headers = {'User-Agent':'Mozilla/5.0 (Windows NT 6.3; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/63.0.3239.132 Safari/537.36'}
data = requests.get("https://jsonplaceholder.typicode.com/comments", headers=headers)
```
$ _ {23.08.03}$<br/><br/>

## **selenium**
js와 같이 동적인 기능이 활용된 페이지에서 데이터를 분류하기 위한 라이브러리  
(지도와 같이 변동성이 클경우 사용)

### ****

```

```

### ****

```

```



$ _ {23.08.04}$<br/><br/>



{% include tag.html tag="python" %}  {% include tag.html tag="bs4" %}  {% include tag.html tag="selenium" %}