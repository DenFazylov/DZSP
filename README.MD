# Это файл для дз. Жду ваши изменения снизу, в последующих строках в этом файле)


# Инструкция по работе в git
## Начало работы c git в VS
GIT - система контроля версий
* Файл -> Открыть папку -> Новая папка
* Вид -> Терминал
* Первое слово (git) - программа к которой обращаешься
* Перемещение осуществляется через cd
* Инициализация - git init -  включение "слежки" за папкой в которой находишься
* Проверка статуса  git status
## *Последовательность работы*
* Создать файл
* Внести изменения
* Сохранить
* git add .
* git commit -m "комментарии"
* git log - просомтр комитов
* q - выход 
* git checkout _ _ _ _ (минимум 4 символа комита) - переход к другой версии
* git checkout main - переход к последней версии файла
* git diff - просмотр изменений (перед git add)

## Ветки
* git branch (название ветки) -  создание ветки
* git branch - прросмотр веток
* git checkout (название ветки) - переход к ветке
* git merge (название ветки)- слияние веток
* git log --graph - графиеский просмотр веток
* git branch -d (название ветки)- удаление ветки (если она слита с основной)
* git branch -D (название ветки)- удалеение ветки (даже если она не слита с основной)

## Работа с удаленными репозиториями
*Как вытащить проект(существующий) из GitHub на комп*
* Создать папку на компе
* В GitHub - зеленая кнопка (Code) - копируем ссылку
* В терминале на компе переходим в созданную папку 
* git clone (ссылка)
* git status
* git log

*Создание связи с GitHub (новый репозиторий)*
* Создать новый репозиторий на GH  
* git remote add origin (адрес нового репозитория)
* git branch -M main  - объявление ветки
* git push -u origin main - "толкнуть" из локального репозитория в удаленный на ветку main

## *Pull request*
    * Fork - репозиторрия другого аккаунта на свой аккаунт в GH
    * создать папку на компе
    * В ней git clone (адрес ссылки со своего аккаунта)
    * Создать новую ветку git branch (название ветки)
    * Перейти на нее черрез git checkout  (название ветки)
    * Внести изменения в проект
    * Закоммитить (как было описано в начале) 
    * Отправить изменения через git push
    * На GH Сравить и отправить через  Compare and Pull request
    * Добавить комментарии при предложении слить