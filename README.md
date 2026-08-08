# AI Wardrobe — лендинг (демо-концепция)

Статический одностраничный сайт: `index.html` + видео `0807.mp4` + фото в `assets/`.
Никакого бэкенда и сборки — открывается прямо в браузере.

## Структура

```
index.html      — сама страница (весь CSS/JS внутри одного файла)
0807.mp4        — видео примерки для hero и Digital Twin
assets/         — стоп-кадры и превью (look-*.jpg, thumb-*.jpg)
```

## Деплой на GitHub Pages

1. Создай новый репозиторий на github.com (например, `ai-wardrobe-landing`) —
   **без** README/`.gitignore`/лицензии, чтобы не было конфликтов при первом пуше.
2. В этой папке выполни (замени `ТВОЙ_ЛОГИН` и название репозитория):

   ```bash
   git init
   git add .
   git commit -m "Initial deploy: AI Wardrobe landing"
   git branch -M main
   git remote add origin https://github.com/ТВОЙ_ЛОГИН/ai-wardrobe-landing.git
   git push -u origin main
   ```

3. На GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**,
   ветка `main`, папка `/ (root)` → **Save**.
4. Через 1–2 минуты сайт будет доступен по адресу вида
   `https://ТВОЙ_ЛОГИН.github.io/ai-wardrobe-landing/`.

Файл называется `index.html` (строго с маленькой буквы) — это обязательное
имя для главной страницы на GitHub Pages, Netlify, Vercel и любом другом
статическом хостинге.

## Альтернатива: Netlify / Vercel (быстрее, без Pages-настроек)

Перетащи эту папку целиком на https://app.netlify.com/drop — сайт получит
рабочую ссылку за несколько секунд, без git и консоли.

## Размер видео

`0807.mp4` ≈ 9,4 МБ — это ниже лимита GitHub на файл (100 МБ) и не требует
Git LFS, коммитится и пушится как обычный файл.
