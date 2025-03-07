---
## Front matter
title: "Лабораторная работа 5"
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

Построение модели эпидемии SIR

# Задание

Получить практические навыки на примерах и выполнить упражнение

# Теоретическое введение

Модель SIR предложена в 1927 г. (W. O. Kermack, A. G. McKendrick). С описанием
модели можно ознакомиться, например в [1].
Предполагается, что особи популяции размера N могут находиться в трёх различ-
ных состояниях:
– S (susceptible, уязвимые) — здоровые особи, которые находятся в группе риска
и могут подхватить инфекцию;
– I (infective, заражённые, распространяющие заболевание) — заразившиеся пере-
носчики болезни;
– R (recovered/removed, вылечившиеся) — те, кто выздоровел и перестал распро-
странять болезнь (в эту категорию относят, например, приобретших иммунитет
или умерших).

# Выполнение лабораторной работы

Строим модель SIR в xcos (рис. [-@fig:001]).

![Схема](image/01.jpg){#fig:001 width=70%}

Вывод графика (рис. [-@fig:002]).

![График](image/02.jpg){#fig:002 width=70%}

Построение модели с помощью блока Modelica (рис. [-@fig:003]).

![Схема](image/03.jpg){#fig:003 width=70%}

Код в openmodelica  и вывод грфика (рис. [-@fig:004]). (рис. [-@fig:005])

![Код](image/04.jpg){#fig:004 width=70%}

![График](image/05.jpg){#fig:005 width=70%}

Задание для самостоятельного выполнения

Схема и график(рис. [-@fig:006])

![Схема и график](image/06.jpg){#fig:006 width=70%}

Схема и график с блоком Modelica (рис. [-@fig:007])

![Схема и график с блоком Modelica](image/07.jpg){#fig:007 width=70%}

Код в OpenModelica (рис. [-@fig:008]).

![Код](image/08.jpg){#fig:008 width=70%}

Графики с различными значениями параметров(рис. [-@fig:009] - [-@fig:012]).

![График](image/09.jpg){#fig:009 width=70%}

![](image/10.jpg){#fig:010 width=70%}

![](image/11.jpg){#fig:011 width=70%}

![](image/12.jpg){#fig:012 width=70%}

# Выводы

В этой лабораторной работе я приобрел навыки построения модели эпидемии SIR

