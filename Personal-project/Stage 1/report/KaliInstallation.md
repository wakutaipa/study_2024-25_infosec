---
## Front matter
title: "Отчёт по индивидуальному проекту"
subtitle: "Установка Kali Linux"
author: "Вакутайпа Милдред"

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
listingTitle: "Листинг"
lofTitle: "Список иллюстраций"
lolTitle: "Листинги"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Получение навыков по установке ОС на менеджер виртуальных машин.

# Задание

Установить дистрибутив Linux.

# Выполнение лабораторной работы

Открываю приложение VirtualBox и создаю новую машину.

![Название машины](image/1.jpg){#fig:001 width=70%}

Создаю виртуальный диск и задаю оперативную память.

![Создание виртуального диска](image/2.jpg){#fig:002 width=70%}

![Объем оперативной памяти](image/3.jpg){#fig:003 width=70%}

Затем соглашаюсь с выбором и запускаю машину.

![Итог](image/4.jpg){#fig:004 width=70%}

Выбираю install чтобы начать установка

![Окно установки](image/5.jpg){#fig:005 width=70%}

При этом замечаю, что образ диска подключен к носителью.

![Подключенный образ](image/6.jpg){#fig:006 width=70%}

Далее выбираю все по моему хотению: Язык установки - английский;

![язык установки](image/7.jpg){#fig:007 width=70%}

Локация - Европа;

![Локация](image/8.jpg){#fig:008 width=70%}

конфигурация клавиатуры (язык).

![конфигурация клавиатуры](image/9.jpg){#fig:009 width=70%}

Настрою сеть. В качестве имени сети задаю мое.

![Настройки сети](image/11.jpg){#fig:010 width=70%}

Создаю пользователя, устанавливаю пароль и настраиваю часы.

![Создание пользователя](image/12.jpg){#fig:011 width=70%}

![Установка пароля](image/14.jpg){#fig:012 width=70%}

![Настройки часов](image/15.jpg){#fig:013 width=70%}

Выбираю диск для работы и сохранния настройки.

![Выбор диска](image/16.jpg){#fig:0014 width=70%}

Далее все настройки сохраняю и устанавливаю систему.

![Установка системы](image/18.jpg){#fig:015 width=70%}

Выбираю окружение рабочий стол и завершаю установки.

![Выбор UI](image/19.jpg){#fig:016 width=70%}

![Завершение установки](image/22.jpg){#fig:017 width=70%}

![Домашний экран](image/23.jpg){#fig:018 width=70%}

Проверяю ,что образ диска пропал, что значит все хорошо устанвлено.

![Пустой носитель](image/24.jpg){#fig:019 width=70%}

# Выводы

Получила навыков по установке ОС на менеджер виртуальных машин.
