---
layout: page
title: Python
subtitle: 5.
menubarcount: 2
menubar: study
menubar2: study_etc_menu
show_sidebar: false
hero_image: /path/to/title.jpg
hero_darken: true
toc: true
toc_title: 목차
---

## shell command
whild card * can use with regex's [] format  

### cd  
```
cd <dir>
cd ..
cd ~
```
* 디렉토리 이동  
* 디렉토리 앞으로 가기  
* 메인 디렉토리로 가기  

<br/>

### mkdir  
```
mkdir <dir_name>
```
* \<dir_name\> 폴더 만들기

<br/>

### touch
```
touch <file_name>
```
* \<file_name\> 파일 만들기

<br/>

### cat
```
cat <file_name>
```
* \<file_name\> 파일 내용보기

<br/>

### mv
```
mv <file_name> <to_dir>
mv <file_name> <to_dir>/<file_name_change>
```
* \<file_name\>을 \<to_dir\>로 이동
* \<file_name\>을 \<file_name_change\>로 이름바꿔서 \<to_dir\>로 이동

<br/>

### cp
```
cp <file_name> <to_dir>
cp <file_name> <to_dir>/<file_name_copy>
```
* \<file_name\>을 \<to_dir\>로 복사
* \<file_name\>을 \<file_name_change\>로 이름바꿔서 \<to_dir\>로 복사

<br/>

### rm
```
rm <file_name>
```
* \<file_name\>을 삭제

<br/>

### vim
```
vim <file_name>
```
* insert mode #i
* insert mode+1 #a
* visual mode #v
    * h - 왼쪽
    * j - 아래
    * k - 위
    * l - 오른쪽
* normal mode #esc
    * dd - delete
    * p - copy
    * :q - quit
    * :q! - force quit
    * :wq - write and quit

$ _ {23.09.15}$<br/><br/>


{% include tag.html tag="python" %}  {% include tag.html tag="" %}