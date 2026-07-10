Вики-документация Orion
Документация для плагина Orion — платное дополнение для FastAsyncWorldEdit (Minecraft).

Ссылка на вики: https://almarelplugins.github.io/orion-docs/

Технический стек
Генератор сайта: MkDocs Material
Хостинг: GitHub Pages (бесплатный, источник — GitHub Actions)
Автосборка: .github/workflows/ci.yml — запускается при push в master
Репозиторий: https://github.com/AlmarelPlugins/orion-docs
Организация: AlmarelPlugins
Как обновить документацию
Открой проект orion-docs в IntelliJ IDEA
Отредактируйте файлы в папке docs/
Ctrl+K → выбор файлов → Зафиксировать и отправить (Commit and Push)
Подожди 1-2 минуты → сайт обновится автоматически
Если сборка упала: github.com/AlmarelPlugins/orion-docs/actions → посмотреть журнал ошибок
Структура проекта
orion-docs/├── mkdocs.yml — отображение MkDocs (меню, тема, навигация)├── README.md — этот файл (техническая справка)├── .github/workflows/│ └── ci.yml — автоматическая сборка и деплой└── docs/ — все страницы документации ├── images/ — изображения для статей ├── index.md — Сообщество (главная) ├── brushes.md — Кисти ├── commands.md — Команды ├── masks.md — Маски ├── patterns.md — Паттерны └── permissions.md — Права доступа

Как добавить новую страницу
Создай новый .md файл в папке docs/ (используй строчные буквы, например new-feature.md)
Добавь его в mkdocs.yml в раздел nav: — без этого страница не появится в меню (путь в mkdocs.yml должен точно совпадать с регистром имени файла)
Commit and Push
Как добавить изображение
Положи картинку в docs/images/ (если папки нет — создай)
В markdown-файле вставь: ![Описание](images/название.png)
Как изменить оформление
Вся настройка внешнего вида — в mkdocs.yml, секция theme:.

Примечания
Язык документации: русский (перевод на английский — позже)
Сайт доступен из РФ без VPN

## Примеры красивых сайтов
https://squidfunk.github.io/mkdocs-material/
https://www.mkdocs.org/
Примеры https://github.com/squidfunk/mkdocs-material/wiki/List-of-community-adaptations

