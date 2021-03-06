# **Инструкция для работы с Markdown в Git**

## ***Установка и настройка Git***
___
1. Устанавливаем Git с оффициального сайта.

2. Устанавливаем Visual Studio Code с оффициального сайта.

3. Создаем рабочую папку (Рекомендуется создавать название папки на английском языке без пробелов).

4. Заходим в VSC и открываем терминал.

5. Задаём имя и email командами:

* git config -­­global user.name "*Имя пользователя*"

* git config ­­-global user.email "*Почта*"

6. Создаём новый фаил с расширением ".md"

7. Создаём репозиторий с помощью команды git init

8. Далее можно начинать работу с файлом (вводим заголовок например).

9. После внесения данных в файл добавляем его к отслеживанию (после сохранения) с помощью команды git add *название файла*

10. С помощью команды git commit -m "*Текст*" сохраняем его и добавляем коментарий к нашей версии документа.

11. Проверяем внеслись ли наши изменения с помощью команды git log

## ***Сводка команд в Git***
___
1. `git init` - позволяет создать репозиторий в выбранной папке.

2. `git add название файла` - добаить файл к отслеживанию (после сохранения файла).

3. `git commit -m "Текст"` - сохранение файла с комментарием.

4. `git diff` - показывает чем отличается текущий файл от изначального.

5. `git log` - показывает все изменения файла.

6. `git checkout номер коммита` (достаточно первых 4 символа коммита) - команда для перехода к нужной версии изменения документа.

7. `git commit -a` -> далее жмём Shift + i -> пишем комментарий -> esc -> Shift + : -> Enter - сохранение файла с большим комментарием, пропуская команду git add).

8. `git commit -a -m "Текст"` - сохранение файла с небольшим коментарием, для мелких изменений файла, пропуская команду git add).

9. `git branch` - показывает ветки файла.

10. `git branch Название ветки` - создание новой ветки.

11. `git checkout Название ветки` - переход на другую ветку.

12. `git commit --amend -m "Новое название коммита"` - Изменение комментария к последнему коммиту.

13. `git status` - отоброжает состояние рабочего каталога и раздела проиндексированных файлов. 

14. `git merge Название ветки` - добавляет изменения данной ветки к необходимой.

15. `git branch -d Название ветки` - удаляет необходимую ветку.

## ***Синтаксис языка Markdown***
___
### *Выделение текста*

* Для выделения текста курсивом обрамляем его звёздочками (*). Например, *Текст*.

* Для выделения текста полужирным обрамляем его двумя звёздочками (**).    Например, **Текст**.

* Для зачёркнутоко текста обрамляем его двумя тильдами (~~). Наприме,  ~~Текст~~.

* Для выделения заголовка в начале строки, перед текстом, добавляем решетку (#). 

* Альтернативный способ выделения текста полужирным или курсивом с помощью нижнего подчёркивания (_). Например, _Полужирный **курсив**_.

### *Списки*

* Чтобы добавить ненумерованные списки, добавляем перед текстом звёздочку (*). Например:
* *Текст*

* Чтобы добавить нумерованные списки, добавляем перед текстом необходимую цифру. Например:
1. *Текст*
2. *Текст*

### *Работа с изображениями*

* Чтобы вставить изображение в текст, необходимо добавить фотографию в рабочую папку и написать следующее:
![Коментарий](*Имя файла с разрешением*)

Например:
![Привет Geek_Brains](GB.png)

### *Ссылки*

Markdown поддерживает два стиля оформления:

* Гиперссылка с немедленным адресом (внутритекстовая).
* Гиперссылка, похожая на сноске.

Для создания внутритекстовой гиперссылки необходимо использовать круглые скобки сразу после закрывающей квадратной. Внутри них необходимо указать URL-адрес. В них же возможно утвердить название, Назначение в кавычки, которое будет назначено назначением, но этот пункт не является обязательным.

[пример](http://example.com/ "Необязательная подсказка")

### *Работа с таблицами*

Таблицы Markdown физически представлены с помощью тире - для разделения строки заголовка из содержимого и трубы | для столбцов. " : " используется для выравнивания столбца. Если вы хотите использовать символ канала ( | ) в содержимом ячейки, вам нужно будет избежать его с помощью обратной косой черты " \ " . Пример таблицы:

Буквы | Цифры | Символы
:---- | :---: | ------:
а     |  1    | @
б     |  2    | $
в     |  3    | \|


### *Цитаты*

Чтобы оформить цитату в markdown, используйте правую угловую скобку. Например:

> Чтобы оформить цитату в markdown, используйте правую угловую скобку.

## ***Работа в GitHub***
___

GitHub - сервис компании Microsoft, который позволяет интегрироваться с программой Git и настроить удаленную работу с репозиториями.

### *Чтобы открыть необходимый репозиторий с Github.com* :

1. Находим необходимый репозиторий на сайте.

2. Нажимаем на зеленную кнопку Code.

3. Копируем ссылку во вкладке HTTPS.

4. С помощью команды `git clone *ссылка*` добавляем репозиторий в VSC

5. Прописываем команду `cd *папку с репозиторием*`

### *Чтобы добавить свой репозиторий на Github.com* :

1. Создаём файл.

2. Создаём аккаунт на сайте.

3. Нажимаем на плюс в правом верхнем углу и New repository.

4. Пишем название репозитория и нажимаем Create repository.

5. Далее выбираем либо создать ноый репозиторий на сайте, либо добавить готовый.

6. Вводим в терминал VSC команды из подсказки выбранного варианта.

7. Проходим авторизацию в всплывающем окне. (если добавляем в первый раз)

8. Теперь можно делиться ссылкой на ваш репозиторий.

9. Чтобы на сайте в репозитории добавились изменения проделанные на вашем локальном репозитории вводим команду `git push`

10. Чтобы в ваш локальный репозиторий добавились все изменения проделанные другими людьми вводим команду `git pull`

### *Чтобы поучаствовать в чужом репозитории на Github.com* :

1. Находим необходимый репозиторий.

2. Нажимаем кнопку Fork в правом верхнем углу, вводим название репозитория и нажимаем Create fork.

3. Копируем ссылку на репозиторий и добавляем в VSC с помощью команды `git clone *ссылка*`

4. Прописываем команду `cd *папку с репозиторием*`

5. Создаём отдельную ветку.

6. Создаём внутри репозитория отдельный файл.

7. Комитим файл.

8. Вносим свои предложения изменений.

9. Вводим команду `git push`

10. На сайте нажимем на кнопку compare & pull request.

11. Добавляем описание к проекту и нажимаем create pull request.


