# Recovery Site — Recovery Agency

Сайт агентства по восстановлению криптоактивов (Canada & Australia).

## Структура проекта

```
recovery-site/
  index.html          ← единственная HTML-страница (все правки только здесь)
  assets/
    img/
      partners/        ← логотипы партнёров
      team/           ← фото команды
      ui/             ← иконки, кнопки, общие элементы интерфейса
  README.md
```

## Куда класть картинки

| Назначение | Папка |
|------------|--------|
| Логотипы партнёров (блок «Partners») | `assets/img/partners/` |
| Фото команды, экспертов | `assets/img/team/` |
| Иконки, кнопки, баннеры, общий UI | `assets/img/ui/` |

## Как называть файлы

- Только латиница, цифры и дефис: `techbullion.png`, `partner-2.png`.
- Без пробелов и спецсимволов.
- Рекомендуемый формат: логотипы и UI — PNG или SVG, фото — JPG/WebP.

Примеры:
- `assets/img/partners/techbullion.png`
- `assets/img/team/lead.jpg`
- `assets/img/ui/logo.svg`

## Как запускать сайт локально

1. Открой папку `recovery-site` в проводнике.
2. Дважды кликни по `index.html` — откроется в браузере по умолчанию.

Или из терминала (из папки `recovery-site`):

```bash
# Windows (PowerShell)
start index.html

# Или запусти простой HTTP-сервер (чтобы всё работало как по HTTP):
npx -y serve .
# затем открой в браузере: http://localhost:3000
```

После добавления картинок в `assets/img/...` используй в `index.html` относительные пути, например:

- `src="assets/img/partners/techbullion.png"`
- `src="assets/img/team/lead.jpg"`
- `src="assets/img/ui/logo.svg"`

## Важно

- **Все изменения вносятся только в `recovery-site/index.html`.**
- Не создавай новые HTML-файлы (index(1).html, new-index.html и т.п.).
