---
# Front matter
lang: ru-RU
title: "Отчёт лабораторной работы №10"
subtitle: "Дисциплина: Операционные системы"
author: "Касьянов Даниил Владимирович"

# Formatting
toc-title: "Содержание"
toc: true # Table of contents
toc_depth: 2
lof: true # List of figures
lot: true # List of tables
fontsize: 12pt
linestretch: 1.5
papersize: a4paper
documentclass: scrreprt
polyglossia-lang: russian
polyglossia-otherlangs: english
mainfont: PT Serif
romanfont: PT Serif
sansfont: PT Sans
monofont: PT Mono
mainfontoptions: Ligatures=TeX
romanfontoptions: Ligatures=TeX
sansfontoptions: Ligatures=TeX,Scale=MatchLowercase
monofontoptions: Scale=MatchLowercase
indent: true
pdf-engine: lualatex
header-includes:
  - \linepenalty=10 # the penalty added to the badness of each line within a paragraph (no associated penalty node) Increasing the value makes tex try to have fewer lines in the paragraph.
  - \interlinepenalty=0 # value of the penalty (node) added after each line of a paragraph.
  - \hyphenpenalty=50 # the penalty for line breaking at an automatically inserted hyphen
  - \exhyphenpenalty=50 # the penalty for line breaking at an explicit hyphen
  - \binoppenalty=700 # the penalty for breaking a line at a binary operator
  - \relpenalty=500 # the penalty for breaking a line at a relation
  - \clubpenalty=150 # extra penalty for breaking after first line of a paragraph
  - \widowpenalty=150 # extra penalty for breaking before last line of a paragraph
  - \displaywidowpenalty=50 # extra penalty for breaking before last line before a display math
  - \brokenpenalty=100 # extra penalty for page breaking after a hyphenated line
  - \predisplaypenalty=10000 # penalty for breaking before a display
  - \postdisplaypenalty=0 # penalty for breaking after a display
  - \floatingpenalty = 20000 # penalty for splitting an insertion (can only be split footnote in standard LaTeX)
  - \raggedbottom # or \flushbottom
  - \usepackage{float} # keep figures where there are in the text
  - \floatplacement{figure}{H} # keep figures where there are in the text
---

# Цель работы

Познакомиться с операционной системой Linux. Получить практические навыки работы с редактором `Emacs`.

# Выполнение лабораторной работы

1. Открываю `emacs` (Рисунок 1).

![](image10/1.png)

(Рисунок 1)

2. Создаю файл lab07.sh с помощью комбинации `Ctrl-x` `Ctrl-f` (Рисунок 2).

![](image10/2.png)

(Рисунок 2)

3. Набираю текст (Рисунок 3):

```
#!/bin/bash
HELL=Hello
function hello {
LOCAL HELLO=World
echo $HELLO
}
echo $HELLO
hello
```

![](image10/3.png)

(Рисунок 3)

4. Сохраняю файл с помощью комбинации `Ctrl-x` `Ctrl-s` (Рисунок 4).

![](image10/4.png)

(Рисунок 4)

5. Проделываю с текстом стандартные процедуры редактирования, используя горячие клавиши.

5.1. Вырезаю целую строку: `Ctrl-k` (Рисунок 5).

![](image10/5.png)

(Рисунок 5)

5.2. Вставляю эту строку в конец файла: `Ctrl-y` (Рисунок 6).

![](image10/6.png)

(Рисунок 6)

5.3. Выделяю область текста: `Ctrl-Space` (Рисунок 7).

![](image10/7.png)

(Рисунок 7)

5.4. Скопирую область в буфер обмена: `Alt-w` (Рисунок 8).

![](image10/8.png)

(Рисунок 8)

5.5. Вставляю область в конец файла: `Ctrl-y` (Рисунок 9).

![](image10/9.png)

(Рисунок 9)

5.6. Вновь выделяю эту область и на этот раз вырезаю её: `Ctrl-w` (Рисунок 10).

![](image10/10.png)

(Рисунок 10)

5.7. Отменяю последнее действие: `Ctrl-/` (Рисунок 11).

![](image10/11.png)

(Рисунок 11)

6. Учусь использовать команды по перемещению курсора.

6.1. Перемещаю курсор в начало строки: `Ctrl-a` (Рисунок 12).

![](image10/12.png)

(Рисунок 12)

6.2. Перемещаю курсор в конец строки: `Ctrl-e` (Рисунок 13).

![](image10/13.png)

(Рисунок 13)

6.3. Перемещаю курсор в начало буфера: `Alt-<` (Рисунок 14).

![](image10/14.png)

(Рисунок 14)

6.4. Перемещаю курсор в конец буфера: `Alt->` (Рисунок 15).

![](image10/15.png)

(Рисунок 15)

7. Управление буферами.

7.1. Вывожу список активных буферов на экран: `Ctrl-x` `Ctrl-b` (Рисунок 16).

![](image10/16.png)

(Рисунок 16)

7.2. Перемещаюсь во вновь открытое окно `Ctrl-x` `o` со списком открытых буферов и переключаюсь на другой буфер (Рисунок 17).

![](image10/17.png)

(Рисунок 17)

7.3. Закрываю это окно `Ctrl-x 0` (Рисунок 18).

![](image10/18.png)

(Рисунок 18)

7.4. Теперь вновь переключаюсь между буферами, но уже без вывода их списка на экран `Ctrl-x b` (Рисунок 19).

![](image10/19.png)

(Рисунок 19)

8. Управление окнами.

8.1. Поделю фрейм на 4 части: разделяю фрейм на два окна по вертикали `C-x 3`, а затем каждое из этих окон на две части по горизонтали `C-x 2` (Рисунок 20).

![](image10/20.png)

(Рисунок 20)

8.2. В каждом из четырёх созданных окон открою новые файлы (Рисунок 21) и введу несколько строк текста (Рисунок 22).

![](image10/21.png)

(Рисунок 21)

![](image10/22.png)

(Рисунок 22)

9. Режим поиска

9.1. Переключусь в режим поиска `Ctrl-s` и найду несколько слов, присутствующих в тексте (Рисунок 23).

![](image10/23.png)

(Рисунок 23)

9.2. Переключусь между результатами поиска, нажимая `Ctrl-s`. У слов появится подсветка (Рисунок 24).

![](image10/24.png)

(Рисунок 24)

9.3. Выйду из режима поиска, нажав `Ctrl-g` (Рисунок 25).

![](image10/25.png)

(Рисунок 25)

9.4. Ставлю курсор в самом начале текста. Перехожу в режим поиска и замены `Alt-%`, ввожу текст, который следует найти и заменить, нажимаю `Enter`, затем ввожу текст для замены. После того как будут подсвечены результаты поиска, нажимаю `!` для подтверждения замены (Рис. 26, 27).

![](image10/26.png)

(Рисунок 26)

![](image10/27.png)

(Рисунок 27)

9.5. Испробую другой режим поиска, нажав `Alt-s o` (Рисунок 28).

Данный вид поиска отличается от обычного тем, что тут считывается строка поиска, которая трактуется как регулярное выражение, и не осуществляется поиск точного совпадения в тексте буфера. Регулярное выражение − это образец, который обозначает набор строк, возможно, и неограниченный набор. 

![](image10/28.png)

(Рисунок 28)

# Контрольные вопросы

3. Контрольные вопросы:

1) `Emacs` − один из наиболее мощных и широко распространённых
редакторов, используемых в мире Unix. По популярности он
соперничает с редактором `vi` и его клонами. В зависимости от ситуации,
`Emacs` может быть:

* текстовым редактором;

* программой для чтения почты и новостей Usenet;

* интегрированной средой разработки (IDE);

* операционной системой и т.д.

Всё это разнообразие достигается благодаря архитектуре `Emacs`,
которая позволяет расширять возможности редактора при помощи
языка `Emacs Lisp`. На языке C написаны лишь самые базовые и
низкоуровневые части `Emacs`, включая полнофункциональный 
интерпретатор языка `Lisp`. Таким образом, `Emacs` имеет встроенный
язык программирования, который может использоваться для настройки,
расширения и изменения поведения редактора. В действительности,
большая часть того редактора, с которым пользователи `Emacs` работают
в наши дни, написана на языке `Lisp`.

2) Основную трудность для новичков при освоении данного редактора
могут составлять большое количество команд, комбинаций клавиш,
которые не получится все запомнить с первого раза и поэтоу придется
часто обращаться к справочным материалам.

3) Буфер – это объект, представляющий собой текст. Если имеется
несколько буферов, то редактировать можно только один. Обычно буфер
считывает данные из файла или записывает в файл данные из буфера.
Окно – это область экрана, отображающая буфер. При запуске редактора
отображается одно окно, но при обращении к некоторым функциям
могут открыться дополнительные окна. Окна `Emacs` и окна графической
среды X Window – разные вещи. Одно окно X Window может быть
разбито на несколько окон в смысле `Emacs`, в каждом из которых
отображается отдельный буфер.

4) Да, можно.
  
5) При запуске `Emacs` по умолчанию создаются следующие буферы:

* `scratch` (буфер для несохраненного текста);

* `Messages` (журнал ошибок, включающий также информацию,
которая появляется в области `EchoArea`);

* `GNU Emacs` (справочный буфер о редакторе).

6) `C-c |`: сначала, удерживая `Ctrl`, нажимаю `c`, после – отпускаю обе
клавиши и нажимаю `|`.

`C-c C-|` сначала, удерживая `Ctrl`, нажимаю `с`, после – отпускаю обе
клавиши и, удерживая `Ctrl`, нажимаю `|`.

7) Чтобы поделить окно на две части необходимо воспользоваться
комбинацией `Ctrl-x 3` (по вертикали) или `Ctrl-x 2` (по горизонтали).

8) Настройки `Emacs` хранятся в файле .emacs.

9) По умолчанию клавиша `←` удаляет символ перед курсором, но в
редакторе её можно переназначить. Для этого необхдимо изменить
конфигурацию файла .emacs.

10)  Более удобным я считаю редактор `emacs`, потому что в нем нет «Командного режима», «Режима ввода», «Режима командной строки», с которыми неудобно работать.

# Выводы

Я познакомился с операционной системой Linux, получил практические навыки работы с редактором `Emacs`.

# Библиография

[Лабораторная работа № 9 - "Текстовой редактор vi"](https://esystem.rudn.ru/mod/resource/view.php?id=718598)

[Лабораторная работа № 10 - "Текстовой редактор emacs"](https://esystem.rudn.ru/mod/resource/view.php?id=718601)