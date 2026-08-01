# spa-orm2

Автономный веб-просмотрщик ORM2-моделей (`.orm`) с отрисовкой диаграмм в нотации **Barker ER**.

## Открыть в браузере

Работает сразу, без настройки репозитория:

**https://htmlpreview.github.io/?https://github.com/zlukfo/spa-orm2/blob/main/orm2-viewer-barker-er-v3.html**

Основной адрес — после включения GitHub Pages (см. ниже):

**https://zlukfo.github.io/spa-orm2/**

> Ссылка вида `github.com/zlukfo/spa-orm2/blob/main/orm2-viewer-barker-er-v3.html` показывает **исходный код**, а не работающую страницу: GitHub отдаёт файлы репозитория с типом `text/plain`, браузер их не исполняет. Чтобы HTML открывался как приложение, нужен хостинг статики.

### Включить GitHub Pages

Один раз в настройках репозитория: **Settings → Pages → Build and deployment → Source: `Deploy from a branch` → Branch: `main`, папка `/ (root)` → Save**.

Через 1–2 минуты заработают адреса:

* https://zlukfo.github.io/spa-orm2/
* https://zlukfo.github.io/spa-orm2/orm2-viewer-barker-er-v3.html

## Локальный запуск

Файл самодостаточен — весь JavaScript и CSS встроены внутрь, внешних зависимостей нет. Достаточно скачать и открыть двойным кликом:

```bash
git clone https://github.com/zlukfo/spa-orm2.git
cd spa-orm2
xdg-open orm2-viewer-barker-er-v3.html   # Linux
# open orm2-viewer-barker-er-v3.html     # macOS
# start orm2-viewer-barker-er-v3.html    # Windows
```

Либо через локальный сервер:

```bash
python3 -m http.server 8000
# затем http://localhost:8000/orm2-viewer-barker-er-v3.html
```

## Состав репозитория

| Файл | Назначение |
| --- | --- |
| `orm2-viewer-barker-er-v3.html` | Приложение целиком: разметка, стили и встроенный скрипт |
| `orm2-viewer-barker-er-v3.js` | Тот же скрипт отдельным файлом — для чтения и правок исходника |
| `index.html` | Точка входа GitHub Pages, перенаправляет на просмотрщик |
| `.nojekyll` | Отключает обработку Jekyll, чтобы Pages отдавал файлы как есть |

## Лицензия

[Apache License 2.0](LICENSE)
