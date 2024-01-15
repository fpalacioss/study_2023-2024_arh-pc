---
## Front matter
title: "Отчет по лабораторной работе №7"
subtitle: "Команды безусловного и условного переходов в Nasm. Программирование
ветвлений"
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

Изучение команд условного и безусловного переходов. Приобретение навыков написания
программ с использованием переходов. Знакомство с назначением и структурой файла
листинга

# Задание

1. Создайте каталог для программам лабораторной работы No 7, перейдите в него и создайте файл lab7-1.asm

2. Введите в файл lab7-1.asm текст программы из листинга 7.1. Создайте исполняемый файл и запустите его.

Измените текст программы в соответствии с листингом 7.2. Создайте исполняемый файл и проверьте его работу.

Измените текст программы добавив или изменив инструкции jmp, чтобы вывод програм-
мы был следующим:
user@dk4n31:~$ ./lab7-1
Сообщение No 3
Сообщение No 2
Сообщение No 1
user@dk4n31:~$

3. Создайте файл lab7-2.asm в каталоге ~/work/arch-pc/lab07. Создайте исполняемый файл и проверьте его работу для разных значений B.

4. Создайте файл листинга для программы из файла lab7-2.asm
nasm -f elf -l lab7-2.lst lab7-2.asm
Откройте файл листинга lab7-2.lst с помощью любого текстового редактора, например
mcedit:
mcedit lab7-2.lst

Откройте файл с программой lab7-2.asm и в любой инструкции с двумя операндами
удалить один операнд. Выполните трансляцию с получением файла листинг

5. Напишите программу нахождения наименьшей из 3 целочисленных переменных 𝑎,𝑏 и . Значения переменных выбрать из табл. 7.5 в соответствии с вариантом, полученным при выполнении лабораторной работы No 7. Создайте исполняемый файл и проверьте его работу.

# Выполнение лабораторной работы

1. Создайте каталог для программам лабораторной работы No 7, перейдите в него и создайте файл lab7-1.asm (рис. @fig:001).

![файл](image/1.jpg){#fig:001 width=70%}

2. Введите в файл lab7-1.asm текст программы из листинга 7.1. Создайте исполняемый файл и запустите его (рис. @fig:002).

![файл](image/2.jpg){#fig:002 width=70%}

Измените текст программы в соответствии с листингом 7.2. Создайте исполняемый файл и проверьте его работу (рис. @fig:003).

![программа](image/2.1.jpg){#fig:003 width=70%}

Измените текст программы добавив или изменив инструкции jmp, чтобы вывод программы был следующим: 
user@dk4n31:~$ ./lab7-1
Сообщение No 3
Сообщение No 2
Сообщение No 1
user@dk4n31:~$ (рис. @fig:004)

![программа](image/2.2.jpg){#fig:004 width=70%}

3. Создайте файл lab7-2.asm в каталоге ~/work/arch-pc/lab07. Создайте исполняемый файл и проверьте его работу для разных значений B (рис. @fig:005).

![файл](image/3.jpg){#fig:005 width=70%}

4. Создайте файл листинга для программы из файла lab7-2.asm
nasm -f elf -l lab7-2.lst lab7-2.asm
Откройте файл листинга lab7-2.lst с помощью любого текстового редактора, например
mcedit:
mcedit lab7-2.lst (рис. @fig:006).

![листинг](image/4.1.jpg){#fig:006 width=70%}

Откройте файл с программой lab7-2.asm и в любой инструкции с двумя операндами
удалить один операнд. Выполните трансляцию с получением файла листинг (рис. @fig:007).

![листинг](image/4.2.jpg){#fig:007 width=70%}

5. Напишите программу нахождения наименьшей из 3 целочисленных переменных 𝑎,𝑏 и . Значения переменных выбрать из табл. 7.5 в соответствии с вариантом, полученным при выполнении лабораторной работы No 7. Создайте исполняемый файл и проверьте его работу (рис. @fig:008).

![программа](image/5.jpg){#fig:0081 width=70%}



# Выводы

Изучены команды условного и безусловного переходов. Приобретены навыки написания программ с использованием переходов. Знакомство с назначением и структурой файла листинга

# Список литературы{.unnumbered}

::: {#refs}
:::
