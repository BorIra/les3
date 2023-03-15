# Инструкция для работы с Git и удалёнными репозиториями

## Что такое Git?
**Git** - это одна из реализаций распределённых систем контроля версий, имеющая как и локальные, так и удалённые репозитории. Является самой популярной реализацией систем контроля версий в мире.

## Подготовка репозитория
Для создание репозитория необходимо выполнить команду *git init* в папке с репозиторием и у Вас создаться репозиторий (появится скрытая папка .git)

# Создание коммитов
## Git add
Для добавления изменений  в коммит используется команда *git add*. Чтобы использовать команду *git add* напишите *git add <имя файла>*.

## Просмотр состояния репозитория
Для того, чтобы посмотреть состояние репозитория используется команда *git status*. Для этого необходимо в папке с репозиторием написать *git status*, и Вы увидите были ли измения в файлах, или их не было.

## Создание коммитов
Для того, чтобы создать коммит(сохранение) необходимо выполнить команду *git commit*. Выполняется она так: *git commit -m "<сообщение к коммиту>*. Все файлы для коммита должны быть ***ДОБАВЛЕНЫ*** и сообщение к коммиту писать ***ОБЯЗАТЕЛЬНО***.

## Перемещение между сохранениями
Для того, чтобы перемещаться между коммитами, используется команда *git checkout*. Используется она в папке с пепозиторием следующим образом: *git checkout <номер коммита>*

## Журнал изменений
Для того, чтобы посмтреть все сделанные изменения в репозитории, используется команда *git log*. Для этого достаточно выполнить команду *git log* в папке с репозиторием

# Ветки в Git
## Создание ветки
Для того, чтобы создать ветку, используется команда *git branch*. Делается это следующим образом в папке с репозиторием: *git branch <название новой ветки>*

## Слияние веток
Для того чтобы дабавить ветку в текущую ветку используется команда *git merge*

## Удаление веток
Для удаления ветки ввести команду *"git branch -d 'name branch'"*


# Домашнее задание

## Выделение текста (emphasis)
Чтобы изменить начертание текста, нужно выделить его с двух сторон спецсимволами следующим образом: <спецсимвол>текст<спецсимвол>.

**Жирный** (bold)
Для выделения текста жирным нужно использовать две звёздочки ** или два нижних подчёркивания __.

*Курсив* (italic)
Для выделения текста курсивом нужно использовать одну звёздочку * или нижнее подчёркивание _.

Обратите внимание, что если вы хотите выделить фрагмент внутри слова, то это корректно сработает только при использовании звёздочек.

~~Зачёркнутый~~ (strikethrough)
Чтобы зачеркнуть текст, нужно использовать две тильды ~~. Такая опция есть только в диалекте GitHub Flavored Markdown.



## Списки (lists)
**Нумерованные** (ordered)
Для создания нумерованного списка перед пунктами нужно поставить число с точкой. При этом нумерация в разметке ленивая. Неважно, какие именно числа вы напишете: Markdown пронумерует список автоматически.
1. Первый
2. Второй
3. Третий

**Ненумерованные** (unordered)

Для создания ненумерованного списка нужно поставить перед каждым пунктом звёздочку *, дефис - или плюс +.
+ первый
+ второй
+ третий

## Цитаты
Для обозначения цитат в языке Markdown используется знак «больше» («>»). Его можно вставлять как перед каждой строкой цитаты, так и только перед первой строкой параграфа. Также синтаксис Markdown позволяет создавать вложенные цитаты (цитаты внутри цитат). Для их разметки используются дополнительные уровни знаков цитирования («>»). Цитаты в Markdown могут содержать всевозможные элементы разметки. Цитаты в языке Markdown выглядят следующим образом:

>Это пример цитаты,
>в которой перед каждой строкой
>ставится угловая скобка.


## Ссылки
Markdown поддерживает два стиля оформления ссылок:

+ Гиперссылка, с немедленным указанием адреса (внутритекстовая);
+ Гиперссылка, подобная сноске.

Подразумевается, что помимо URL-адреса существует еще текст ссылки. Он заключается в квадратные скобки. Для создания внутритекстовой гиперссылки необходимо использовать круглые скобки сразу после закрывающей квадратной. Внутри них необходимо поместить URL-адрес. В них же возможно расположить название, заключенное в кавычки, которое будет отображаться при наведении, но этот пункт не является обязательным.

[пример](http://gb.ru/ "GeekBrains")

При ссылке на локальную директорию возможно использование относительного пути (от текущей страницы, сайта и т.п.)

Markdown поддерживает упрощённый порядок автоматического создания ссылок для URL-адресов и адресов электронной почты. Для этого достаточно поместить URL-адрес или почтовый адрес в угловые скобки, и Markdown сделает его гиперссылкой. В отличие от вышеописанных стилей, в данном случае сам же URL-адрес или почтовый адрес становится и текстом гиперссылки. Автоматические ссылки на адреса электронной почты работают аналогично.

<http://gb.ru/>

## Изображения
В Markdown существует 2 способа вставки изображений в документ. Рассмотрим спобоб с помощью непосредственного указания URL-адреса изображения. Синтаксис данной команды выглядит следующим образом:
+ восклицательный знак;
+ квадратные скобки, в которых указывается альтернативный изображению текст (он станет содержимым атрибута в элементе img);
+ круглые скобки, содержащие URL-адрес или относительный путь изображения, а также (необязательно) всплывающую подсказку, заключённуе в двойные или одиночные кавычки.

![Букет ландышей](/landyshi.jpg)

## Таблицы
В Markdown есть возможность оформлять таблицы. Столбцы разделяются вертикальными линиями | , а строка с шапкой отделяется от остальных дефисами - , которых можно ставить сколько угодно.

 Header column 1| Header column 2
 ----------- | ----------- 
 some text | more text 
 some text | more and longer text 

html table:

 <table>
     <tr>
       <td>Header column 1</td>
        <td>Header column 2</td>
    <tr>
    <tr>
        <td>some text</td>
        <td>more text</td>
    </tr>
    <tr>
        <td>some text</td>
        <td>more and longer text</td>
    </tr>
 </table>