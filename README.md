# figma

### 1. Настройка Git

0. git config --global user.name "Ваше Имя"        # Установка имени
0. git config --global user.email "ваш@email.com"  # Установка email
0. git config --list                              # Проверить настройки


0. git clone https://github.com/username/repo.git  # Склонировать репозиторий
0. cd repo                                        # Перейти в папку проекта

### 3. Основной рабочий цикл

0. git status                     # Проверить изменения
0. git add .                      # Добавить ВСЕ изменения
0. git add file.txt               # Добавить конкретный файл
0. git commit -m "Описание"       # Закоммитить изменения
0. git push origin main           # Отправить изменения на GitHub
0. git pull                       # Обновить локальную версию

### 4. Ветки (branches)

0. git branch                      # Показать все ветки
0. git branch new-feature          # Создать новую ветку
0. git checkout new-feature        # Переключиться на ветку
0. git checkout -b new-feature     # Создать и переключиться
0. git merge new-feature           # Влить ветку в текущую (например, в main)
0. git push origin new-feature     # Отправить ветку на GitHub

### 5. Отмена изменений

0. git restore file.txt           # Отменить изменения в файле (до add)
0. git reset --hard HEAD          # Отменить ВСЕ изменения (осторожно!)
0. git commit --amend             # Исправить последний коммит

### 6. Работа с удалённым репозиторием (GitHub)

0. git remote -v                  # Показать подключённые репозитории
0. git remote add origin URL      # Добавить удалённый репозиторий
0. git push -u origin main        # Первая отправка (с привязкой ветки)
0. git fetch                      # Проверить изменения на GitHub
0. git pull origin main           # Скачать и объединить изменения

### 7. Просмотр истории

0. git log                        # Показать историю коммитов
0. git log --oneline              # Краткая история
0. git diff                       # Показать изменения

### 8. Дополнительно
bash
git stash                      # Временно сохранить изменения
git stash pop                  # Вернуть сохранённое
git tag v1.0                   # Создать тег (версию)
git push --tags                # Отправить теги на GitHub

##Пример рабочего процесса:

###Клонируем репозиторий:

bash
git clone https://github.com/user/project.git
cd project
Создаём новую ветку:

bash
git checkout -b feature/login
Вносим изменения, сохраняем:

bash
git add .
git commit -m "Добавлена форма входа"
git push origin feature/login
После проверки вливаем в main через Pull Request на GitHub.
