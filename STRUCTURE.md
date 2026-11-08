# Структура проекта

```
game/
├── index.html          ← основной лендинг (править сюда)
├── code.html           ← устаревший / исходный экспорт; не источник правды
├── server.js           ← static file server (PORT=5173)
├── package.json        ← npm start → node server.js
├── DESIGN.md           ← дизайн-система Acid Paper Editorial
├── AGENTS.md           ← инструкции для AI
├── STRUCTURE.md        ← этот файл
├── screen.png          ← визуальный референс
└── assets/
    └── anna-orlova.png ← фото Анны Орловой (секция #about)
```

## `index.html` — секции сверху вниз

| # | Комментарий в коде | Якорь / id | Содержание |
|---|--------------------|------------|------------|
| — | header + mobile menu | `#mobile-menu`, `#menu-toggle` | Нав: игры / метод / обо мне / отзывы / цены |
| 1 | HERO | (без id) | Заголовок «А ЕСЛИ МОЖНО ИНАЧЕ?», CTA, `#labyrinth-board` |
| 2 | ACID MARQUEE | — | Бегущая строка |
| 3 | INTERACTIVE BENTO | `#interactive-selector` | Карточки запроса `.query-card` → `#diagnostic-result` |
| 4 | HOW IT WORKS | `#how-it-works` | Фазы / как проходит игра |
| 5 | WITH WHAT QUERY | нет id | 6 направлений терапии (bento) |
| 6 | TRANSFORM RESULTS | нет id | Что уносишь с игры |
| 7 | PRICING & FORMATS | `#formats` | Тарифы: группа / 1:1 / … + LeadPay |
| 8 | ABOUT AUTHOR | `#about` | Анна Орлова + `assets/anna-orlova.png` |
| 9 | REVIEWS | `#reviews` | Отзывы (`#reviews-carousel`) |
| 10 | FAQ | `#faq` | Аккордеон `.faq-item` |
| 11 | FINAL CTA | нет id | Финальный призыв + WhatsApp |
| — | footer | — | Ссылки, контакты, дисклеймер |

### Ключевые якоря для нав / CTA

- `#interactive-selector` — «найти свою игру»
- `#how-it-works` — «как это работает»
- `#formats` — тарифы
- `#about` — об авторе
- `#reviews` — отзывы
- `#faq` — вопросы

## Диагностика запросов (секция 3)

Карточки `data-card-id="0"…"6"` вызывают `selectRequest(index)`.

Данные в массиве `queryData` (внизу `index.html`):

| index | Тема рекомендации |
|------:|-------------------|
| 0 | Отношения и близость |
| 1 | Точка призвания |
| 2 | Стратегия достижений |
| 3 | Освобождение |
| 4 | Источник энергии |
| 5 | Бизнес-тренинг «Масштаб» |
| 6 | Точка ноль // Навигатор |

Результат пишется в `#result-tag`, `#result-title`, `#result-desc`, `#result-link`.

Чекауты LeadPay (сейчас в коде):

- `…/checkout/1817/` — большинство игр
- `…/checkout/1737/` — часть сценариев (достижения / энергия)

## Стили и motion

- Tailwind config inline (`#tailwind-config`) — токены из `DESIGN.md`
- Кастомный CSS в `<style>`: marquee, maze, stamp, slam, protocol-blink и т.д.
- Классы motion: `.reveal-stamp`, `.phase-card`, `.sticker-live`, `.maze-path`, `[data-count]`

## `server.js`

Отдаёт файлы из корня проекта. `/` → `index.html`. Path traversal блокируется. MIME по расширению.

## `code.html` vs `index.html`

| | `index.html` | `code.html` |
|--|--------------|-------------|
| Статус | live | архив / черновик |
| Motion / UX | расширен (stamp, maze draw, counters, reduced-motion) | базовая версия |
| Отзывы | grid / обновлённый layout | горизонтальный scroll |
| Размер | ~1375 строк | ~1144 строк |

При сомнении всегда смотри и правь `index.html`.
