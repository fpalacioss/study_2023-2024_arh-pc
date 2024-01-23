---
## Front matter
title: "Отчет по лабораторной работе №10"
subtitle: "Работа с файлами средствами Nasm"
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

Приобретение навыков написания программ для работы с файлами.

# Задание

1. Создайте каталог для программам лабораторной работы No 10, перейдите в него и создайте файлы lab10-1.asm, readme-1.txt и readme-2.txt

2. Введите в файл lab10-1.asm текст программы из листинга 10.1 (Программа записи в файл сообщения). Создайте исполняемый файл и проверьте его работу.

3. С помощью команды chmod измените права доступа к исполняемому файлу lab10-1,запретив его выполнение. Попытайтесь выполнить файл. Объясните результат.

4. С помощью команды chmod измените права доступа к файлу lab10-1.asm с исходным текстом программы, добавив права на исполнение. Попытайтесь выполнить его и объясните результат.

5. В соответствии с вариантом в таблице 10.4 предоставить права доступа к файлу readme-1.txt представленные в символьном виде, а для файла readme-2.txt – в двочном виде. Проверить правильность выполнения с помощью команды ls -l.

6. Напишите программу работающую по следующему алгоритму:
• Вывод приглашения “Как Вас зовут?”
• ввести с клавиатуры свои фамилию и имя
• создать файл с именем name.txt
• записать в файл сообщение “Меня зовут”
• дописать в файл строку введенную с клавиатуры
• закрыть файл
Создать исполняемый файл и проверить его работу. Проверить наличие файла и его содержимое с помощью команд ls и cat
 
# Выполнение лабораторной работы

1. Создайте каталог для программам лабораторной работы No 10, перейдите в него и создайте файлы lab10-1.asm, readme-1.txt и readme-2.txt (рис. @fig:001).

![файлы](image/1.jpg){#fig:001 width=70%}
 
2. Введите в файл lab10-1.asm текст программы из листинга 10.1 (Программа записи в файл сообщения). Создайте исполняемый файл и проверьте его работу (рис. @fig:002).

![lab10-1](image/2.jpg){#fig:002 width=70%}

3. С помощью команды chmod изменили права доступа к исполняемому файлу lab10-1, запретив его выполнение. Попытались выполнить файл. Отказано в доступе(рис. @fig:003).

![запрет выполнения](image/3.jpg){#fig:003 width=70%}

4. С помощью команды chmod изменили права доступа к файлу lab10-1.asm с исходным текстом программы, добавив права на исполнение. Результат - файл не предназначен для исполнения (рис. @fig:004).

![права на исполнение lab10-1.asm](image/4.jpg){#fig:004 width=70%}

5. В соответствии с вариантом в таблице 10.4 предоставили права доступа к файлу readme-1.txt представленные в символьном виде, а для файла readme-2.txt – в двочном виде. Проверили правильность выполнения с помощью команды ls -l (рис. @fig:005).

![права доступа](image/5.jpg){#fig:005 width=70%}

6. Написали программу. Создали исполняемый файл и проверили его работу. Проверили наличие файла и его содержимое с помощью команд ls и cat
(рис. @fig:006), (рис. @fig:007)

![работа программы](image/6.1.jpg){#fig:006 width=70%}

![ls cat](image/6.2.jpg){#fig:007 width=70%}

# Выводы

Приобретены навыки написания программ для работы с файлами.

# Список литературы{.unnumbered}

::: {#refs}
:::
