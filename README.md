# Ben & Tech Cat Assets

Набор пиксель-арт ассетов и документации для персонажей Ben и Tech Cat.

## Структура

```text
/assets
  /ben
    /fullbody      # фулл-боди спрайты Бэна
    /portraits     # портреты / аватары Бэна
    /stickers      # стикеры Бэна (прозрачный фон)
  /cat
    /fullbody      # фулл-боди спрайты кота
    /portraits     # портреты / аватары кота
    /stickers      # стикеры кота (прозрачный фон)
  /both
    /scenes        # сцены с Бэном и котом
    /banners       # баннеры / обложки
  /ui
    /icons         # иконки для интерфейса
    /emojis        # маленькие эмодзи-версии
/docs
  canon-doc.md     # канон: палитра, стиль, позы, тех.правила
  prompts_short.md # короткие промпты под частые задачи
  usage-guide.md   # где и как использовать ассеты
  custom_prompts.md# кастомные промпты под конкретные картинки

```


Базовые правила
```text
  • Базовый канвас персонажей: 128×128 px.
  • Масштабирование только целыми множителями (x2/x3/x4) и только Nearest Neighbor.
  • Сцены и баннеры собираются из уже масштабированных спрайтов.
  • Фон:
  • сцены/баннеры: тёмный (#05030A или близкий);
  • стикеры/эмодзи: прозрачный.
```

Детали по стилю и использованию — в /docs.


---

## 4. Как стартануть (пошагово)

1. Создай пустой репозиторий на GitHub: `ben-tech-cat-assets`.
2. Локально:

```bash
git clone git@github.com:YOUR_USERNAME/ben-tech-cat-assets.git
cd ben-tech-cat-assets

mkdir -p assets/ben/{fullbody,portraits,stickers}
mkdir -p assets/cat/{fullbody,portraits,stickers}
mkdir -p assets/both/{scenes,banners}
mkdir -p assets/ui/{icons,emojis}
mkdir docs


