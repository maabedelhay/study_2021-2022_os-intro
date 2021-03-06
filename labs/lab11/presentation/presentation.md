---
## Front matter
lang: ru-RU
title: Программирование в командном процессоре ОС UNIX. Ветвления и циклы
author: Абд эль хай мохамад
institute: RUDN University, Moscow, Russian Federation
date: 28 Мая 2022

## Formatting
toc: false
slide_level: 2
theme: metropolis
header-includes: 
 - \metroset{progressbar=frametitle,sectionpage=progressbar,numbering=fraction}
 - '\makeatletter'
 - '\beamer@ignorenonframefalse'
 - '\makeatother'
aspectratio: 43
section-titles: true
---

# Вступление
В этой лаборатории я написал 4 программы bash. Идея состоит в том, чтобы автоматизировать определенные задачи с помощью скрипта bash. Это основная причина использования bash. Программы содержали более сложные программные решения. Например, использование массивов, условных циклов и логического оператора в стиле bash.

```bash
[ ! -z $N ] && echo "Not equal to zero" 
```
будет работать только в том случае, если условная команда выполнена успешно "вернул код выхода 0". он будет работать так же, как и второй способ, но лучше.

```bash
if [[ ! -z $N ]]
then 
  echo "Not equal to zero"
fi
```
# Задание
## №1
Программа, которая ищет шаблоны и использует аргументы для подсчета строк или для входного и выходного файла.

## №2
Программа C, которая принимает входное число. Оцените его, а затем отправьте введенное число в ОС с помощью функции exit(). Вторая программа с bash прочитает код выхода программы, которая содержит введенное число, а затем напечатает его.

## №3
Программа для создания числовых файлов. В качестве аргумента передается число. и если файлы уже существуют удалит их.

## №4
Программа, которая сжимает файлы из указанного каталога. Только те файлы, которые последний раз изменялись более 7 дней назад.

# Выполнение задание

- №1. Использовал команду getopts и grep. С помощью команды getopts я создал аргументы команды, которые позволяют пользователю взаимодействовать с программой и указывать различные параметры. 
  
- №2. Программа C для проверки введенного числа, если оно меньше, больше или равно 0. Отправьте введенное число с помощью функции exit () «exit (inpouted number)». Файл Bash прочитает код выхода программы C и распечатает его. Это оно.

## Выполнение задание

- №3. Создан сценарий bash, который будет принимать два аргумента: имя файла и количество файлов для создания. Если файлы уже существуют, они будут удалены, а если нет, будут созданы.
 
- №4. Команда tar будет сжимать файлы из указанного каталога. Только файлы, которые последний раз изменялись более 7 дней.



# Вывод
Скрипт Bash может делать удивительные вещи. Сложные программы bash могут выполнять такие действия, как резервное копирование каталога, синхронизация данных с удаленных веб-сайтов или с ними, простые программы с графическим интерфейсом и многое другое.

## {.standout}

Спасибо
