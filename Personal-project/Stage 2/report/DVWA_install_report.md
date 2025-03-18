---
## Front matter
title: "Отчет по Второму Этапу Индивидуального Проекта "
subtitle: "Установка DVWA"
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
lofTitle: "Список иллюстраций"
## Misc options
indent: true
header-includes:
  - \usepackage{indentfirst}
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Получить практические навыки по установке DVWA.

# Задание

1. Установить DVWA.

# Выполнение лабораторной работы

Открою github и захожу в репозиторий dvwa и копирую ссылку.

![репзиторий DVWA ](image/1.jpg){#fig:001 width=70%}

Открою терминал, и с помощью cd, вхожу в директорию html, где сохраняются файлы локального хоста. В этой же директории клонирую репозиторий.

![Клонирование DVWA в /html](image/2.jpg){#fig:002 width=70%}

С помощью ls поверяю, что клонирование было успешно и потом разрешаю все права на все файлы в DVWA используя chmod -R 777

![chmod -R 777](image/3.jpg){#fig:003 width=70%}

Проверяю работу и захожу в dvwa/config, чтобы настроить веб-приложение.

![директория config](image/4.jpg){#fig:004 width=70%}

Далее копирую config.int.php который содержит конфигурацию приложения.

![копирование config.int.php](image/5.jpg){#fig:005 width=70%}

В этом файле изменяю пароль, имя пользователя на  mwaku и создаю базу данных waku и сохраняю изменения.

![редактирование файла конфигурации](image/6.jpg){#fig:006 width=70%}

Запускаю mysql с помощью start mysql и проверяю используя status mysql.

![Запуск mysql](image/7.jpg){#fig:007 width=70%}

![прверка работы mysql](image/8.jpg){#fig:008 width=70%}

Далее я вхожу в mmysql используя mysql -u root -p 

![вход в mysql](image/9.jpg){#fig:009 width=70%}

Создаю базу данных waku и нового пользователя используя create user 'mwaku'@'127.0.0.1' identified by 'password'. Используя эту команду, создала пользователя mwaku, работаюшего на сервер локального хоста (127.0.0.1) и пароль password.

![создание пользоателя](image/10.jpg){#fig:0010 width=70%}

Разрешаю все правав доступа этому пользователю к базе данных и завершаю работы.

![Разрешение права](image/11.jpg){#fig:0011 width=70%}

Запускаю сервер apache2.

![Запуск apache2](image/12.jpg){#fig:0012 width=70%}

Далее вхожу в /etc/php/8.2. 

![вход в /etc/php/8.2](image/13.jpg){#fig:0013 width=70%}

Включаю значения allow_url_fopen и allow_url_include в файле apache2/php.ini.

![Включение  allow_url](image/14.jpg){#fig:0014 width=70%}

Перезапускаю сервер apache2 испоьзуя systemctl restart apache2. 

![Перезапуск apache2](image/15.jpg){#fig:0015 width=70%}

Открою 127.0.0.1./dvwa/setup.php в браузере.   

![страница веб-приложения](image/16.jpg){#fig:0016 width=70%}

Нажимаю кнопку create/Reset database. Создается базу данных и мне перенаправляют на страницу входа. Вхожу используя логин admin и пароль p@ssword.

![Вход в DVWA](image/17.jpg){#fig:0017 width=70%}

После входа попадаем на домашнюю страницу dvwa.

![Домшняя страница dvwa](image/18.jpg){#fig:0018 width=70%}


# Выводы

Получила навыки по установке DVWA.

# Список литературы{.unnumbered}

[Set up DVWA in Kali Linux][https://akshaygupta21.medium.com/how-to-setup-dvwa-in-kali-linux-e7c0dc272bba]
