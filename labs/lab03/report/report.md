---
## Front matter
title: "Лабораторная работа 3"
subtitle: "Имитационное моделирование"
author: "Голощапов Ярослав Вячеславович"

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
mainfont: IBM Plex Serif
romanfont: IBM Plex Serif
sansfont: IBM Plex Sans
monofont: IBM Plex Mono
mathfont: STIX Two Math
mainfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
romanfontoptions: Ligatures=Common,Ligatures=TeX,Scale=0.94
sansfontoptions: Ligatures=Common,Ligatures=TeX,Scale=MatchLowercase,Scale=0.94
monofontoptions: Scale=MatchLowercase,Scale=0.94,FakeStretch=0.9
mathfontoptions:
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

Моделирование стохастических процессов

# Задание

Получить практические навыки на примерах и выполнить упражнение

# Теоретическое введение

M |M |1 — однолинейная СМО с накопителем бесконечной ёмкости. Поступаю-
щий поток заявок — пуассоновский с интенсивностью λ. Времена обслуживания
заявок — независимые в совокупности случайные величины, распределённые по
экспоненциальному закону с параметром μ.

# Выполнение лабораторной работы

Реализация модели СМО (рис. [-@fig:001]). (рис. [-@fig:002]).

![Реализация модели](image/01.jpg){#fig:001 width=70%}

![Вывод](image/02.jpg){#fig:002 width=70%}

В каталоге с проектом создал отдельный файл graph_plot и добавил код соблюдая синтаксис (рис. [-@fig:003]) .

![graph_plot](image/03.jpg){#fig:003 width=70%}

Упражнение: Сделайте файл исполняемым. После компиляции файла с проектом, запустите
скрипт в созданном файле graph_plot, который создаст файл qm.pdf с результата-
ми моделирования (рис. [-@fig:004]) (рис. [-@fig:005])

![Файл исполняемый](image/04.jpg){#fig:004 width=70%}

![Результаты моделирования](image/05.jpg){#fig:005 width=70%}


# Выводы

В этой лабораторной работе я научился моделировать стохастические процессы

