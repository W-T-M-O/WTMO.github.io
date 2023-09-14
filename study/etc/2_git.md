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

git config --global --list
```
autocrlf 문자 개행 세팅(줄바꿈)

## 깃 원격지 설정
```
git remote add <origin_name> <git_repo>
```

## 깃 작업 내역 확인
```
git status
```

## 깃 다음 버전에서 팔로우업 할 파일 추가
```
git add <file_name>
```

## 깃에 팔로우업한 파일 기준으로 새로운 버전을 생성 및 설명추가
```
git commit -m "<message>"
```

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



{% include tag.html tag="git" %}