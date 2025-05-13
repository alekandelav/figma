# figma

### 1. Настройка Git

#. git config --global user.name "Ваше Имя"        # Установка имени
#. git config --global user.email "ваш@email.com"  # Установка email
#. git config --list                              # Проверить настройки

### 2. Клонирование репозитория
bash
git clone https://github.com/username/repo.git  # Склонировать репозиторий
cd repo                                        # Перейти в папку проекта

### 3. Основной рабочий цикл
bash
git status                     # Проверить изменения
git add .                      # Добавить ВСЕ изменения
git add file.txt               # Добавить конкретный файл
git commit -m "Описание"       # Закоммитить изменения
git push origin main           # Отправить изменения на GitHub
git pull                       # Обновить локальную версию

### 4. Ветки (branches)
bash
git branch                      # Показать все ветки
git branch new-feature          # Создать новую ветку
git checkout new-feature        # Переключиться на ветку
git checkout -b new-feature     # Создать и переключиться
git merge new-feature           # Влить ветку в текущую (например, в main)
git push origin new-feature     # Отправить ветку на GitHub

### 5. Отмена изменений
bash
git restore file.txt           # Отменить изменения в файле (до add)
git reset --hard HEAD          # Отменить ВСЕ изменения (осторожно!)
git commit --amend             # Исправить последний коммит

### 6. Работа с удалённым репозиторием (GitHub)
bash
git remote -v                  # Показать подключённые репозитории
git remote add origin URL      # Добавить удалённый репозиторий
git push -u origin main        # Первая отправка (с привязкой ветки)
git fetch                      # Проверить изменения на GitHub
git pull origin main           # Скачать и объединить изменения

### 7. Просмотр истории
bash
git log                        # Показать историю коммитов
git log --oneline              # Краткая история
git diff                       # Показать изменения

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
