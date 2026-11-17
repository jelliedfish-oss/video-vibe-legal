# Video Vibe — app information website

Двуязычный landing приложения Video Vibe: главная, Privacy Policy, Terms of Use и Help & Support. Хостинг — GitHub Pages из `main`, папки `/`.

- English: https://jelliedfish-oss.github.io/video-vibe-legal/en/
- Русский: https://jelliedfish-oss.github.io/video-vibe-legal/ru/
- Разделы: `/{en,ru}/privacy/`, `/{en,ru}/terms/`, `/{en,ru}/help/`.
- Прежний адрес `/privacy/` сохранён для совместимости.

Пока во всех разделах стоит явный текст-заглушка. Юридические тексты ещё не опубликованы.

## Как добавить текст

Откройте соответствующий файл `en/{privacy,terms,help}.md` или `ru/{privacy,terms,help}.md`, замените include на согласованный Markdown-текст и добавьте в front matter `content_status: published`. Пока статус pending, страница не индексируется. Общие подписи находятся в `_data/translations.yml`; шаблон — `_layouts/default.html`, оформление — `assets/styles.css`.

Сайт использует Jekyll GitHub Pages; внешние шрифты, аналитика и JavaScript не добавлены. При смене домена/репозитория обновите `url` и `baseurl` в `_config.yml`. Внутренние ссылки учитывают baseurl.
