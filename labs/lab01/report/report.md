---
## Front matter
title: "Шаблон отчёта по лабораторной работе №1"
subtitle: "Простейший вариант"
author: "Шияпова Дарина Илдаровна"

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

Целью данной работы является приобретение практических навыков установки операционной системы на виртуальную машину, настройки минимально необходимых для дальнейшей работы сервисов.

# Задание

Установить ОС на виртуальную машину, выполнить минимальную настройку и получить некоторую информацию.  


# Выполнение лабораторной работы

Так как операционную систему мы установили и настроили еще в первом семестре, то сразу можем переходить к выполнению домашнего задания.

Получим информацию о версии ядра Linux (рис. @fig:001).

![Команда dmesg | grep -i "Linux version" ](/home/dishiyapova/Изображения/Снимки экрана/11.png){#fig:001 width=70%}

Получим информацию о частоте процессора  и его модели(рис. @fig:002).

![Команда dmesg | grep -i "pricessor" и  Команда dmesg | grep -i "CPU0"  ](/home/dishiyapova/Изображения/Снимки экрана/12.png){#fig:002 width=70%}

Получим информацию о доступном объеме оперативной памяти (рис. @fig:003).

![Команда dmesg | grep -i "memory" ](/home/dishiyapova/Изображения/Снимки экрана/13.png){#fig:003 width=70%}

Получим информацию о последовательности монтирования файловых систем.(рис. @fig:004).

![Команда dmesg | grep -i "mounted" ](/home/dishiyapova/Изображения/Снимки экрана/15.png){#fig:004 width=70%}

Получим информацию о типе гипервизора.(рис. @fig:005).

![Команда dmesg | grep -i "mounted" ](/home/dishiyapova/Изображения/Снимки экрана/14.png){#fig:005 width=70%}


# Выводы

При выполнении лабораторной работы номер 1 мы научились устанавливать и настраивать виртуальную машину, а также находить различную информацию о системе.

# Список литературы{.unnumbered}

::: {#refs}
:::
