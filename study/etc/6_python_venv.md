---
layout: page
title: Python
subtitle: 6.
menubarcount: 2
menubar: study
menubar2: study_etc_menu
show_sidebar: false
hero_image: /path/to/title.jpg
hero_darken: true
toc: true
toc_title: 목차
---

## venv(normal setting, makedir it self)

python -m venv <venv_name>   

source <venv_name>/bin/activate # mac   

source <venv_name>/Script/activate # git bash with window   

Scripts\activate.bat # cmd with window   

deactivate   

## pipenv(not makedir it self)
pip install pipenv   

python -m pipenv --python <version>   

python -m pyenv versions # 여기에 버전들 깔림   

python -m pipenv shell   

exit   

* pipenv --venv  
* pipenv --py  
* pipenv run python # 가상환경으로 파이썬 실행하기  

### jupyter setting

pip install jupyter  

pip install ipykernel  

python -m ipykernel install — user — name 가상환경이름  

jupyter kernelspec list  

jupyter kernelspec uninstall 가상환경이름  


$ _ {23.09.15}$<br/><br/>



{% include tag.html tag="python" %}