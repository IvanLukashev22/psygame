# PSYGAME — контекст для агента

Лендинг трансформационных психологических игр Анны Орловой. Один статический сайт без фреймворка, бандлера и бэкенд-логики.

## С чего начинать

1. Читай `STRUCTURE.md` — карта файлов, секций и якорей.
2. Дизайн-токены и визуальные правила — `DESIGN.md` (neo-brutal / editorial).
3. **Рабочий источник правды по UI — `index.html`**, не `code.html`.

## Стек

| Часть | Что используется |
|--------|-------------------|
| Разметка | Один большой `index.html` (HTML + CSS + JS inline) |
| Стили | Tailwind CDN (`cdn.tailwindcss.com`) + кастомный `<style>` |
| Шрифты | Dela Gothic One (дисплей), Onest (текст), Material Symbols |
| Сервер | `server.js` — простой static HTTP на порту `5173` |
| Запуск | `npm start` → `http://127.0.0.1:5173` |

## Правила правок

- Правь **`index.html`**. `code.html` — старый/черновой снимок; не синхронизировать без явной просьбы.
- Не выносить в React/Vite/отдельные модули, пока пользователь сам не попросит.
- Сохраняй neo-brutal язык: hard shadows, `0` radius, borders 2–4px, палитра paper / ink / acid / cobalt / tomato.
- Движение — «штамп / slam / pulse», не мягкие AI-fade. Учитывать `prefers-reduced-motion`.
- Оплата и CTA ведут на LeadPay (`app.leadpay.ru/checkout/...`) и WhatsApp/Telegram — не ломать ссылки без замены.
- Текст сайта на русском; тон прямой, редакционный, без эзотерики.

## Где лежит логика

Всё интерактивное — внизу `index.html` в `<script>`:

- `queryData` + `selectRequest(i)` — диагностика запросов → рекомендация игры
- `initGameMotion()` — maze draw, stamp reveals, счётчики
- `toggleFaq` / `toggleMobileMenu` — аккордеон и мобильное меню

## Ассеты

- `assets/anna-orlova.png` — фото автора
- `screen.png` — референс/скрин макета
- `DESIGN.md` — дизайн-система (не править ради «красоты кода»)
