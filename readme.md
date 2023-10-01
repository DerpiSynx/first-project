# Первый файл формата readme
---
## Проверака знаний
---
### Курсив и жирный текст
 С помощью `*` и `_` можно выделить текст курсивом. Например *Курсив* или _Курсив_
 С помощью `_ _` можно выделить текст жирным шрифтом. Например __Жирный шрифт__
 Эти 2 выделения можно объединить. Например __*Жирный курсив*__
### Разные заголовки
 С помощью знака `#` можно создавать заголовки разных размеров. Чем больше знаков `#` тем меньше заголовок.
 Например
 # Большой заголовкок
 ## *Средний заголовок с курсивом*
 ### __Маленький заголовок с жирным шрифтом__
---
### Программный код
 С помощью знака ````` можно вставить в файл программный код. Например
 ```python
 str privet = Hello world
 print (privet)
 ```
### Ссылки
 Также в файл readme можно вставить ссылки.
 Для этого нужно написать слово, которое будет ссылкой в квадратных скобках, после этого должна быть ссылка в круглых скобках.
 Например
 [Яндекс](www.yandex.ru)
### Хэши
Хэш это уникальный определитель коммита, обычно состоит из __40 символов__. Цифрами от 0 до 9 и английскими буквами верхнего и нижнего регистра.
Хэш можно увидеть при вызове лога.
### Логи
 Лог это список всех коммитов и информации о них(Хэш, автор, время, сообщение).
 Комманда - git log
 Краткий лог выводит сокращенный хэш, которого достаточно для уникального определения коммита в рамках репозитория и сообщение.
 Команда - git log --oneline
 Также есть параметр Head, который ссылается на последний коммит  
### GIT статусы
 У файла в репозитории может быть несколько статусов
 Untracked - git знает о файле но никак не следит за ним
 Tracked - файл был закомичен хотя бы 1 раз
 Staged - файл был добавлен командой git add
 Modified - после команды git add файл был еще раз изменен.

 Более сложная версия
 ```mermaid

 ``` 
 