---
title: "Working with gh-pages from RStudio"
author: "Sergey Bushmanov"
date: "08/27/2014"
output: html_document
---


# Как создать gh-pages ветку в GitHub репозитории

1. Создать соотвествующий репозиторий в GitHub.
2. Создать проект в RStudio.
3. Сделать первый коммит.
4. В командной строке в домашней директории проекта:


```r
git branch gh-pages
```

5. Создать файл в корне рабочей диретокрии .nojekyll


```r
file.create(".nojekyll")
```

6. Сделать коммит.


```r
git push origin gh-pages
```

7. Добавить в  "./.git/config"


```r
[branch "gh-pages"]
        remote = origin
	merge = refs/heads/gh-pages
```

