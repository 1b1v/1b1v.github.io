# Вики-документация Orion

Внутренняя техническая справка для поддержки и обновления документации плагина **Orion** — премиум-дополнения для FastAsyncWorldEdit (Minecraft).

- 🌐 **Ссылка на вики:** [https://almarelplugins.github.io/orion-docs/](https://almarelplugins.github.io/orion-docs/)
- 💻 **Репозиторий:** [AlmarelPlugins/orion-docs](https://github.com/AlmarelPlugins/orion-docs)

---

## Технический стек
*   **Генератор сайта:** MkDocs Material (с кастомным Full-Bleed Two-Tone дизайном).
*   **Хостинг:** GitHub Pages (бесплатный).
*   **Автосборка:** CI/CD через GitHub Actions (`ci.yml`) — запускается при push в `master`.

---

Структура проекта
orion-docs/
├── mkdocs.yml                 # Конфигурация MkDocs (меню, тема, плагины)
├── README.md                  # Эта техническая справка
├── .github/workflows/
│   └── ci.yml                 # Автоматическая сборка и деплой
└── docs/                      # Все страницы документации
    ├── images/                # Изображения для статей
    ├── stylesheets/
    │   └── custom.css         # CSS для визуального разделения экрана
    ├── index.md               # Главная (Community)
    ├── brushes.md             # Кисти
    ├── commands.md            # Команды
    ├── masks.md               # Маски
    ├── patterns.md            # Паттерны
    └── permissions.md         # Права доступа

🛠 Руководство по работе
Как обновить документацию
Открой проект orion-docs в IntelliJ IDEA.
Отредактируй нужные .md файлы в папке docs/.
Нажми Ctrl+K → выбери файлы → Commit and Push.
Подожди 1-2 минуты → сайт обновится автоматически.
Если сайт не обновился, проверь журнал ошибок: GitHub Actions
Для проверки изменений нажми Ctrl + F5 на сайте (сброс кэша браузера).
Как добавить новую страницу
Создай новый файл .md в папке docs/ (используй строчные буквы, например new-feature.md).
Добавь его в файл mkdocs.yml в раздел nav: (путь должен точно совпадать с регистром имени файла!). Без этого страница не появится в левом меню.
Сделай Commit and Push.
Как добавить изображение
Положи картинку в папку docs/images/.
В markdown-файле вставь код: ![Описание картинки для SEO](images/название.png)
Как добавить Логотип сайта
Положи квадратное изображение logo.png в папку docs/images/.
Открой файл mkdocs.yml.
В разделе theme: найди и раскомментируй (удали #) две строки:
YAML

logo: images/logo.png
favicon: images/logo.png
Сделай Commit and Push.
Как изменить оформление
Настройка цветов, иконок и логики работы — в mkdocs.yml, секция theme:.
Тонкая настройка верстки (шрифты, отступы, фон) — в docs/stylesheets/custom.css.
📌 Примечания
Язык документации: Английский (адаптировано под технические стандарты комьюнити FAWE).
Сайт доступен из РФ без VPN.

## Примеры красивых сайтов
https://squidfunk.github.io/mkdocs-material/
https://www.mkdocs.org/
Примеры https://github.com/squidfunk/mkdocs-material/wiki/List-of-community-adaptations

