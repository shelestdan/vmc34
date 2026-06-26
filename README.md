# VMC static site

Статичный сайт для Timeweb: загрузить содержимое этой папки в `public_html`.

## Файлы

- `index.html` - вся структура и текст.
- `style.css` - дизайн и адаптив.
- `assets/img/` - локальные оптимизированные изображения.
- `.htaccess` - безопасное gzip/cache правило для Apache.
- `robots.txt`, `sitemap.xml` - базовая индексация.

## Проверка локально

```bash
python3 -m http.server 8080
```

Открыть `http://localhost:8080`.

## Важно

Форма намеренно заменена на `mailto:`. Для маленького тарифа Timeweb это надежнее, чем PHP-обработчик без антиспама.
