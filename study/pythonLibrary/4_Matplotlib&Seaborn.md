---
layout: page
title: Python
subtitle: 1.
menubarcount: 2
menubar: study
menubar2: study_pythonLibrary_menu
show_sidebar: false
hero_image: /path/to/title.jpg
hero_darken: true
toc: true
toc_title: 목차
---
## **Matplotlib**
파이썬 시각화 라이브러리로 matlab을 참고하여 제작함.
주로 논문에서 figure를 작성할때 사용함.
> * pyplot  
> 빠르고 간단하게 그래프를 그릴때 사용  
> * OOP-style  
> 구체적으로 요소들을 손봐서 그래프를 그릴때 사용

### **pyplot**
아래 3개와 같이 기본적인 형이 존재하며 추가적인 속성들을 변경하여 그래프를 그린다.

* 단일 plot 생성
```
plt.figure()  
plt.plot()  
plt.show()  
```
* 단일 plot에 그래프들 겹치기
```
plt.figure()  
plt.plot()  
plt.plot()  
plt.show()  
```
* 다중 plot 작성
```
plt.figure()  
plt.subplot(<axis0 size>,<axis1 size>,<position num>)
plt.subplot(<axis0 size>,<axis1 size>,<position num>)
plt.show()  
```  

다음과 같은 데이터가 있을때  
```
x = ["data1", "data2", "data3", "data4"]  
y = [111, 156, 487, 445]  
z = [50, 549, 450, 42]  
```

plt.plot(x,y, label="plot")  

plt.title("Title", fontdict={'fontsize': 10}, loc="center")  
plt.xlabel("menu", fontdict={'fontsize': 10}, loc="left")  
plt.ylabel("data", fontdict={'fontsize': 10}, loc="bottom")  
plt.bar(x, y, width=0.2, label="bar")  
plt.legend(loc="upper right")  
plt.yticks([1,2,5,50,100,200])  
plt.ylim(0, 1000)  
plt.barh()  
plt.grid(alpha=1, color="red", linewidth=10)  
plt.scatter(y,z, color="red", marker="^")  

plt.show()  

plt.figure(figsize=(10,5))  

plt.subplot(2,1,1)  
plt.bar(x, y, width=0.2, label="bar")  
plt.subplot(2,1,2)  
plt.scatter(np.random.rand(1,100),np.random.rand(100), color="red", marker="^")  

plt.show()




## Seaborn(Statisical Data Visualization library based on Matplotlib)
Matplotlib를 참고하여 제작하였으나 파이썬의 라이브러리에 더 친화적이다.  
pandas의 dataframe을 사용하는데 용이함




$ _ {23.07.25}$<br/><br/>



{% include tag.html tag="python" %}  {% include tag.html tag="" %}