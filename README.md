# Инструкция по привязке сайта к домену denginazad.online (Рег.ру)

В архиве находятся готовые файлы для публикации на домене `denginazad.online`:
- `index.html` — главная страница приложения «РационБюджет»
- `CNAME` — файл привязки домена `denginazad.online` (для GitHub Pages / Surge)
- `netlify.toml` и `vercel.json` — конфигурации для Netlify и Vercel
- `manifest.json` и `robots.txt` — служебные файлы веб-приложения

## Быстрый запуск на Netlify (за 2 минуты без терминала)
1. Войдите на netlify.com и перетащите распакованную папку со всеми файлами в окно **Deploys**.
2. Перейдите в **Domain management** → **Add a domain** и укажите `denginazad.online`.
3. В личном кабинете Рег.ру откройте **Домены** → `denginazad.online` → **DNS-серверы и управление зоной** → **Изменить**.
4. Убедитесь, что выбраны серверы `ns1.reg.ru` и `ns2.reg.ru`, нажмите **Добавить запись**:
   - Тип `A` | Subdomain: `@` | IP Address: `75.2.60.5`
   - Тип `CNAME` | Subdomain: `www` | Canonical name: `<имя-вашего-проекта>.netlify.app.`
