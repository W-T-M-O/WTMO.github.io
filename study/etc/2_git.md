---
layout: page
title: etc
subtitle: 2.git
menubarcount: 2
menubar: study
menubar2: study_etc_menu
show_sidebar: false
hero_image: /path/to/title.jpg
hero_darken: true
toc: true
toc_title: 목차
---


## 깃 글로벌 셋팅
```
git config --global core.autocrlf input # mac
git config --global core.autocrlf true # win
git config --global user.name "name"
git config --global user.email "email"
git config --global core.editor "vim" # editor를 vim으로 세팅
git config --global core.pager "cat" # pager를 cat으로 세팅
git config --global --list
```
autocrlf 문자 개행 세팅(줄바꿈)
shell에서 vim ~/.gitconfig로 수동 변경가능

## 깃 원격지 설정
```
git remote add <origin_name> <git_repo>
git remote -v
```
* 원격지 세팅
* 원격지 종류 확인

## 깃 작업 내역 확인
```
git status
```

## 파일 내부 작성자 확인
```
git blame <file_name>
```

## 깃 clone
```
git clone <url>
git clone <url> <dir>
```
* 깃 가져오기
* 깃 \<dir\>에 가져오기

## 깃 다음 버전에서 팔로우업 할 파일 추가
```
git add <file_name>
```

## 깃에 팔로우업한 파일 기준으로 새로운 버전을 생성 및 설명추가
```
git commit -m "<message>"
git commit --amend
```
* 깃 easy 커밋
* 직전 커밋 수정

<!-- ## 깃에 팔로우업한 파일 기준으로 새로운 버전을 생성 및 설명추가
```
git commit -m "<message>"
git commit --amend
```
* 깃 easy 커밋
* 직전 커밋 수정 -->

## 현재 깃의 버전 로그 확인
```
git log
git reflog
```
* 전체 로그확인
* 하드 리셋한 로그까지 확인

## 깃 브랜치 관리
```
git branch
git branch -a
git branch <name>
git branch -d <name>
git branch -r
```
* 브랜치 리스트
* 브랜치 원격지 포함 리스트
* 브랜치 생성
* 브랜치 삭제
* 원격지 브랜치 확인

## 깃 브랜치 변경
```
git checkout <name>
git checkout -t <origin_name>
```
* 브랜치 변경
* 원격지 브랜치로 변경

## 깃 병합
```
git merge <name>
```
\<name\>을 현재 브랜치로 합치기

## 깃 리셋
```
git reset --hard HEAD~<num>
git reset --hard <commit_name>
```
* HEAD를 \<num\>횟수만큼 되돌아간다.
* HEAD를 \<commit_name\>으로 되돌아간다.

## 깃 복구
```
git reset --hard ORIG_HEAD
```
* HEAD를 기존의 ORIG_HEAD로 되돌린다.

## 깃 태그 관리
```
git tag <tag_name>
git tag <tag_name> <commit_id>
git push origin <tag_name>
git push --tags
git tag -d <tag_name>
git push origin :tags/<tag_name>
git tag -l "<tag_name>"
```
* 태그 생성
* 특정 커밋에 태그 생성
* 특정 태그 원격에 업로드
* 태그 전체 원격에 업로드
* 로컬 특정 태그 삭제
* 원격 특정 태그 삭제
* 태그 확인

$ _ {23.08.17}$<br/><br/>

## conventional commit  

[example](https://www.conventionalcommits.org/ko/v1.0.0)

1. commit 제목은 구나 절의 형태로 나타내기

2. capitalize 중요

3. prefix(type) 달기
    - feat : 기능 개발 관련
    - fix : 오류 개선, 버그 패치
    - docs : 문서화 작업
    - test : test관련
    - conf : 환경설정 관련
    - build : 빌드 작업 관련
    - ci : continuous integration 관련
    - chore : 패키지 매니저, 스크립트
    - style : 코드 포매팅 관련
    - refactor : refactoring 작업

example

> {type}:{description} 작업단위 축약(if ! after type mean breaking change happen)  
> {body} 작업 상세 기술  
> {footer} 부가정보(ex) BREAKING CHANGE:drop social login support

### pre-commit
commit을 하는데 있어서 통일 된 규격의 파일을 원격지에 올리기 위한 방법
```
pip install pre-commit

pre-commit sample-config > .pre-commit-config.yaml
cat .pre-commit-config.yaml

pre-commit run

pre-commit run -a

pre-commit install
```

$ _ {23.09.15}$<br/><br/>

{% include tag.html tag="git" %}