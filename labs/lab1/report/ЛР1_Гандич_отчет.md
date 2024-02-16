---
## Front matter
title: "Отчёт по лабораторной работе №1."
subtitle: "Установка и конфигурация операционной системы на виртуальную машину"
author: " Гандич Дарья Владимировна. НБИбд-02-22."

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

# Выполнение лабораторной работы

1. Через консоль открываем Virtual Box

![открываем Virtual Box](image/1.png){ #fig:001 width=90% }

2. Настраиваем в свойствах VirtualBox месторасположение каталога для виртуальных машин.

![месторасположение каталога](image/2.png){ #fig:002 width=90% }

3. Копируем диск с дистрибутивом в папку с именем, оттуда указываем этот диск в носители.

![носитель дистрибутива](image/3.png){ #fig:003 width=90% }

![установка носителя](image/4.png){ #fig:004 width=90% }

4. Запускаем машину, создаем нужные настройки согласно описанию лабораторной работы. 

![настройка машины](image/5.png){ #fig:005 width=90% }

5. Ждем установки.

![установка](image/6.png){ #fig:006 width=90% }

6. После завершения установки, перезапускаем машину. Входим в систему, совершаем команды из текста лабораторной работы.

![вход в ос](image/7.png){ #fig:007 width=90% }

7. Выполняем команду dmesg  и dmesg | less

![dmesg](image/8.png){ #fig:008 width=90% }

![dmesg | less](image/9.png){ #fig:009 width=90% }

8. Выполняем домашнюю работу, используя команду dmesg | grep -i "то, что ищем"

![dmesg | grep -i](image/10.png){ #fig:010 width=90% }

# Вывод
Мы установили операционную систему Rocky на виртуальную машину. Настроили сервисы для минимальной необходимой работы.

::: {#refs}
:::
