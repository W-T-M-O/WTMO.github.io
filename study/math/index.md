---
layout: page
title: Math
subtitle: Getting Starteddsd
menubar: study_math_menu
show_sidebar: false
hero_image: /path/to/title.jpg
# primary: true
hero_darken: true
# hide_hero: true
toc: true
toc_title: Custom Title
---

### **부분집합(subset) 상호 포함(double inclusion)**

집합$A$와 집합 $B$가 있을때 $A$에 있는 원소가 모두 $B$에 소속이 된다면 이를 $A$가 $B$의 **부분집합(subset)**이라고 부르며$a^2 + b^2 = \leq c^2$이라고 표기한다. $A$와 $B$가 서로의 부분집합일 경우 **상호 포함(double inclusion)**상태라고 부른다.

---
<blockquote>
Ut venenatis, nisl scelerisque sollicitudin fermentum, quam libero hendrerit ipsum, ut blandit est tellus sit amet turpis.</blockquote>

{% highlight python linenos %}
YOUR CODE HEREsdasfsafsafasfasfsfsfs
sdfds
sdfsdf
dsf
{% endhighlight %}

**합집합(union)($\cup$)** : $A \cup B := {\{ x \in X : x \in A \ or \ x \in B}\}$

**교집합(intersection)(**$\cap$**)** : $A \cap B := {\{ x \in X : x \in A \ and \ x \in B}\}$

**차집합(set minus)(**$\setminus$**)** : $A-B =A \setminus B := {\{ x \in X : x \in A \ but \ x \notin B}\}$

**여집합(complement)(**$X^C$**)** : $A^c := X \setminus A$

**곱집합(cartesian product)(**$\times$**)** : $A \times B := {\{ (a,b) : a \in A \ and \ b \in B}\}$


## General Configuration

Much of a Jekyll's configuration is held in the `_config.yml` file in the project root. 

For information on general Jekyll configuration, please check out the [Jekyll docs](https://jekyllrb.com/docs/configuration/).

Below are some specific options that you might want to set in your `_config.yml` when using Bulma Clean Theme.

## Lang

The html lang attribute is set to `en` by default but you can override this in the _config.yml file `lang: en`

## Direction
The html _dir_ attribute is set to `ltr` by default. It can be overridden in the _config.yml file like `direction: rtl`. 

## Google Analytics 

To enable Google Analytics add `google_analytics: UA-xxxxxxxx` to your `_config.yml` replacing the UA-xxxxxxxx with your Google Analytics property.

```yaml
google_analytics: UA-xxxxxxxx
```

## GitHub Sponsor

If you have a GitHub sponsors account set up, you can add your username to `gh_sponsor` in the `_config.yml` file and it will display a link to your profile on the right of the navbar.

```yaml
gh_sponsor: chrisrhymes
```

Further information on Sponsors feature available in the [Sponsors docs page](/bulma-clean-theme/docs/sponsors/).

## Disqus

Disqus comments are available for posts. To be able to use them, you need to set your disqus shortname in `_config.yml`. 
```
disqus.shortname=<example-com.disqus.com>  
```

Need help finding your Disqus Shortname?  [See this helpful post by Disqus on the matter.](https://help.disqus.com/en/articles/1717111-what-s-a-shortname)  

Then you need to set your Jekyll environment to production: 

```JEKYLL_ENV=production bundle exec jekyll build```. 

Post comments are enabled by default if disqus is enabled. If you want to disable comments on a specific post, set the following in the post's front matter: 

```markdown
comments: false
```