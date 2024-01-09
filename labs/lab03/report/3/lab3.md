---
## Front matter
title: "Отчет по лабораторной работе №3"
subtitle: "Дисциплина архитектура компьютера"
author: "Паласиос Фелипе"

## Generic otions
lang: ru-RU
toc-title: "Содержание"

## Bibliography
bibliography: bib/cite.bib
csl: pandoc/csl/gost-r-7-0-5-2008-numeric.csl

## Pdf output format
toc: true # Table of contents
toc-depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4
documentclass: scrreprt
## I18n polyglossia
polyglossia-lang:
  name: russian
  options:
	- spelling=modern
	- babelshorthands=true
polyglossia-otherlangs:
  name: english
## I18n babel
babel-lang: russian
babel-otherlangs: english
## Fonts
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase,Scale=0.9
## Biblatex
biblatex: true
biblio-style: "gost-numeric"
biblatexoptions:
  - parentracker=true
  - backend=biber
  - hyperref=auto
  - language=auto
  - autolang=other*
  - citestyle=gost-numeric
## Pandoc-crossref LaTeX customization
figureTitle: "Рис."
tableTitle: "Таблица"
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lotTitle: "Список таблиц"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Целью работы является освоение процедуры оформления отчетов с помощью легковесного
языка разметки Markdown.

# Задание

1. Откройте терминал

2. Перейдите в каталог курса сформированный при выполнении лабораторной работы
No2:
cd ~/work/study/2023-2024/"Архитектура компьютера"/arch-pc/
Обновите локальный репозиторий, скачав изменения из удаленного репозитория с помо-
щью команды git pull

3. Перейдите в каталог с шаблоном отчета по лабораторной работе No 3
cd ~/work/study/2023-2024/"Архитектура компьютера"/arch-pc/labs/lab03/report

4. Проведите компиляцию шаблона с использованием Makefile. Для этого введите ко-
манду make
При успешной компиляции должны сгенерироваться файлы report.pdf и report.docx.
Откройте и проверьте корректность полученных файлов.

5. Удалите полученный файлы с использованием Makefile. Для этого введите команду
make clean
Проверьте, что после этой команды файлы report.pdf и report.docx были удалены.

6. Откройте файл report.md c помощью любого текстового редактора, например gedit
gedit report.md
Внимательно изучите структуру этого файла.
Архитектура ЭВМ

7. Заполните отчет и скомпилируйте отчет с использованием Makefile. Проверьте кор-
ректность полученных файлов. (Обратите внимание, для корректного отображения
скриншотов они должны быть размещены в каталоге image)

8. Загрузите файлы на Github.
cd ~/work/study/2023-2024/"Архитектура компьютера"/arch-pc
git add .
git commit -am 'feat(main): add files lab-3'
git push


# Выполнение лабораторной работы

1. Открываю терминал и перехожу в рабочий каталог arch-pc и обновляю репозиторий с помощью команды git pull (рис. @fig:001).

![каталог arch-pc и обновляю репозиторий с помощью команды](image/1.jpg){#fig:001 width=70%}

2. Перехожу в каталог с шаблоном отчета по лабораторной работе №3 и выполняю компиляцию  (рис. @fig:002).

![переход в каталог](image/2.jpg){#fig:002 width=70%}
 
3. Проверяю выполнилась ли компиляция (рис. @fig:003).

![компиляция шаблона reoprt](image/3.jpg){#fig:003 width=70%}

4. Выполняю удаление новых компилированных файлов и сразу проверяю удаление.

5. Открываю файл report.md с помощью текстового редактора и делаю отчет по лабораторной работе.

6. Откройте файл report.md c помощью любого текстового редактора, например gedit
gedit report.md
Внимательно изучите структуру этого файла.
Архитектура ЭВМ

7. Заполните отчет и скомпилируйте отчет с использованием Makefile. Проверьте кор-
ректность полученных файлов. (Обратите внимание, для корректного отображения
скриншотов они должны быть размещены в каталоге image)

8. Загрузите файлы на Github.
cd ~/work/study/2023-2024/"Архитектура компьютера"/arch-pc
git add .
git commit -am 'feat(main): add files lab-3'
git push

# Выводы

Были получены навыки по работе с языком разметки Markdown

# Список литературы{.unnumbered}

::: {#refs}
:::
