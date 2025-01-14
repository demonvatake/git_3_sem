# git_3_sem

# Инструкция для работы с MarkDown

Заходишь такой в документ и открываешь его а этот, документ предназначен для ознакомления пользователя с функциональными возможностями языка разметки Markdown. Markdown – это облегченный язык разметки, который является инструментом преобразования кода в HTML. Главной особенностью данного языка является максимально простой синтаксис, который служит для упрощения написания и чтения кода разметки, что, в свою очередь, позволяет легко его корректировать. Теперь рассмотрим более подробно функции языка разметки Markdown.

Markdown не является заменой HTML. Синтаксис Markdown достаточно ограничен, и соответствует лишь небольшому подмножеству элементов HTML. Он включает в себя следующие элементы:

## Выделение текста

Чтобы выделить текст курсивом необходимо обрамить его звездочками (*) или знаком  нижнего подчеркивания (_), Например, *вот так* или _вот так_.

Чтобы выделить текст полужирным, необходимо обрамить его двойными звездочками (**) или двойным знаком нижнего подчеркивания (__). Например, **вот так** или __вот так__.

Альтернативные способы выделения текста жирным или курсивом нужны для того, чтобы мы могли совмещать оба этих способа. Например, _текст может быть выделен курсивом и при этом может быть **полужирным**_.

## Списки



Чтобы добавить ненумерованные списки, необходимо пункты выделить звездочкой (*), Например вот так:
* Элемент 1
* Элемент 2
* Элемент 3

Чтобы добавить нумерованные списки, необходимо пункты просто пронумеровать Например, вот так:
1. Первый пункт
2. Второй пункт

## Работа с изображениями

Чтобы вставить изображение в текст, достаточно написать следующее:
![Пример](картинка.jpg)

## Ссылки

Ссылки
Markdown поддерживает два стиля оформления ссылок:

Гиперссылка, с немедленным указанием адреса (внутритекстовая);
Гиперссылка, подобная сноске.
Подразумевается, что помимо URL-адреса существует еще текст ссылки. Он заключается в квадратные скобки. Для создания внутритекстовой гиперссылки необходимо использовать круглые скобки сразу после закрывающей квадратной. Внутри них необходимо поместить URL-адрес. В них же возможно расположить название, заключенное в кавычки, которое будет отображаться при наведении, но этот пункт не является обязательным.

  [пример](http://example.com/ "Необязательная подсказка")
В результате на экран выводится следующее: пример При ссылке на локальную директорию возможно использование относительного пути (от текущей страницы, сайта и т.п.)

При создании сносной гиперссылки вместо целевого адреса используется вторая пара квадратных скобок, внутри которых помещается метка, идентификатор ссылки (id).

[пример][id]:
Также, можно использовать пробел, чтобы отделять 2 пары квадратных скобок:

[пример] [id]: 
В этом случае возможно определить идентификатор в любом месте документа:

[id]: http://example.com/ "Необязательная подсказка"
В результате на экран выводится следующее: [пример] [id] [id]: http://example.com/ "Необязательная подсказка" Иными словами, она состоит из следующих элементов:

Идентификатор ссылки, окружённый квадратными скобками (которым может предшествовать необязательный отступ от одного до трёх пробелов);
Двоеточие;
Один или несколько пробелов (или символов табуляции);
URL гиперссылки;
Необязательный заголовок (подсказка к изображению, которая всплывает при наведении на него) гиперссылки, заключённый либо в двойные или одиночные кавычки, либо в скобки.
Идентификаторы ссылок могут состоять из букв, цифр, пробелов и знаков пунктуации, однако они не чувствительны к регистру. То есть эти два варианта эквивалентны:

[текст ссылки][a]
[текст ссылки][A]
Markdown позволяет также использовать неявно выраженный идентификатор (сокращенный). В этом случае метка не приводится, вместо неё текст гиперссылки используется и в качестве её имени, а вторая пара квадратных скобок остаётся пустою. Например, чтобы сделать слово «Example» гиперссылкой, ведущей на сайт http://example.com/, достаточно написать:

[Example][]
и затем определить гиперссылку:

[Example]: http://example.com/
В результате на экран выводится следующее: [Example][] [Example]: http://example.com/

## Работа с таблицами

## Цитаты
Для обозначения цитат в языке Markdown используется знак «больше» («>»). Его можно вставлять как перед каждой строкой цитаты, так и только перед первой строкой параграфа. Также синтаксис Markdown позволяет создавать вложенные цитаты (цитаты внутри цитат). Для их разметки используются дополнительные уровни знаков цитирования («>»). Цитаты в Markdown могут содержать всевозможные элементы разметки. Цитаты в языке Markdown выглядят следующим образом:

>Это пример цитаты,
>в которой перед каждой строкой
>ставится угловая скобка.

>Это пример цитаты,
в которой угловая скобка
ставится только перед началом нового параграфа.
>Второй параграф.
Вложение цитаты в цитату выглядит следующим образом:

> Первый уровень цитирования
>> Второй уровень цитирования
>>> Третий уровень цитирования
>
>Первый уровень цитирования
В результате на экран выводится следующее:

Это пример цитаты, в которой перед каждой строкой ставится угловая скобка.

Это пример цитаты, в которой угловая скобка ставится только перед началом нового параграфа.

Второй параграф.

Вложенная цитата:

Первый уровень цитирования

Второй уровень цитирования

Третий уровень цитирования

Первый уровень цитирования

Уровень цитирования не может превышать 15-й.
## Заключение
Более подробно можно ознакомится на сайте

[Сайт_с_синтаксисом](https://gist.github.com/Jekins/2bf2d0638163f1294637#Blockquotes)

Полезные ссылки:

Официальный сайт [GitHub](https://github.com/);
Синтаксис [Markdown](https://gist.github.com/Jekins/2bf2d0638163f1294637#Blockquotes).


Коммит, созданный нами, хранится в репозитарии, привязанном к конкретной папке на нашем компьютере, т.е. является локальным. Это полезно, если мы работаем над проектом самостоятельно. Однако в большинстве случаев возникает необходимость обеспечить доступ к результатам работы или доставить код на сервер, где он будет выполняться.



Как подключиться к удаленному репозитарию?


Для загрузки данных в удаленный репозитарию сначала нужно к нему подключиться. В нашем примере мы используем адрес https://github.com/tutorialzine/awesome-project, однако пользователь может создать собственный удаленный репозитарий на GitHub, BitBucket или другом подобном сервисе. Это занимает некоторое время, однако в дальнейшем полностью себя оправдывает, тем более, что подобные службы имеют пошаговые инструкции для правильно выполнения нужных действий.



Для того, чтобы связать созданный нами локальный репозитарий с удаленным, выполним такую команду:

# This is only an example. Replace the URI with your own repository address.
$ git remote add origin https://github.com/tutorialzine/awesome-project.git


Первая строка напоминает нам, что URI репозитария, который приведен в примере, нужно изменить на свой.



Иногда бывает так, что проект имеет несколько удаленных репозитариев – в таком случае каждому из них присваивается собственное имя. Главный репозитарий принято называть origin.



Как отправить изменения в удаленный репозитарий?


Теперь, когда у нас в локальном репозитарии создан коммит и мы подключились к удаленному, можем отправить его на сервер. Мы это будем делать каждый раз, когда хотим обновить данные в удаленном репозитарии.



Отправка коммита осуществляется с помощью команды push, которая имеет два параметра - имя удаленного репозитория (в нашем случае origin) и ветку, в которую необходимо внести изменения (master — это ветка по умолчанию для всех репозиториев).

$ git push origin master
Counting objects: 3, done.
Writing objects: 100% (3/3), 212 bytes | 0 bytes/s, done.
Total 3 (delta 0), reused 0 (delta 0)
To https://github.com/tutorialzine/awesome-project.git
* [new branch] master -> master


Если мы все сделали правильно, то отправленный файл hello.txt на удаленном сервере мы можем увидеть с помощью браузера. Важный момент – некоторые сервисы для отправки изменений могут требовать дополнительной аутентификации.



Как клонировать удаленный репозитарий?


Если у других пользователей возникла необходимость клонировать удаленный репозитарий, они могут получить полностью работоспособную копию при помощи команды clone:

$ git clone https://github.com/tutorialzine/awesome-project.git


GitHub автоматически создаст новый локальный репозитарий в виде удаленного на собственном сервере.



Как запросить изменения с удаленного репозитария?


В случае, если другим пользователям нет необходимости делать клон удаленного репозитария, а нужно просто получить информацию об изменениях, это можно сделать с помощью команды pull:

$ git pull origin master
From https://github.com/tutorialzine/awesome-project
* branch master -> FETCH_HEAD
Already up-to-date.