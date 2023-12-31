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


Можно сделать такую схему. 

 ```mermaid
graph LR;
  untracked -- "git add" --> staged;
  staged    -- "???"     --> tracked/comitted;

%% стрелка без текста для примера: 
  A --> B;
 ``` 
### Изменение коммита
 С помощью команды
 git --amend
 
 --amend - означает изменить последний коммит
 
 --no-edit - такая приписка означает не менять комментарий

 -m - такая приписка означает поменять комментарий
 
 Команда --amend без флагов включит редактор для редактирования сообщения вручную. (Nano)Ctrl+x сохраняет сообщение.(Vim) Esc, :qa!, Enter

 git reset -hard <Хэш коммита> удаляет все коммиты после указанного. Файлы также откатываются до версии этого коммита.
 
 git restore <file> вернет файл к последней версии сохраненной командой git add или git commit
### Команды(разные)
git cat <file> - выводит содержимое файла

git diff - изменения в файле сейчас и в предыдущем коммите. --staged изменения в файле в последнем коммите и в версии staged

get diff <Хэш> <Хэш> - покажет все изменения между коммитами

echo <Текст> - выводит текст на экран . echo <Текст> >> <file> добавляет текст на новую строку в файл. echo <Текст> > <file> далит содержимое файла и добавит новый текст
