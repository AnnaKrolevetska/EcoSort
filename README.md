# EcoSort — mobile web app

HTML-версія мобільного застосунку EcoSort, зібрана з макету Figma. Чистий HTML/CSS/JS — без збірки, без залежностей.

## Що всередині

```
index.html             весь застосунок (екрани, стилі, логіка)
assets/                зображення з Figma (Земля-маскот, баки, пляшка, нагороди) + іконки
manifest.webmanifest   щоб сайт можна було «встановити» на телефон як застосунок
sw.js                  офлайн-кеш
```

## Екрани

Splash → онбординг (3 слайди, свайп) → реєстрація / вхід → EcoHome → EcoProfile,
EcoMap (фільтри, точки, картка пункту з маршрутом у Google Maps), Scanner (можна зробити фото камерою телефона),
Item Details → нагорода +10 EP, EcoLearn → кольори баків / відео / квіз, EcoPoints.

Бали, кількість предметів та історія зберігаються в браузері (localStorage).
На телефоні застосунок відкривається на весь екран, на комп'ютері — у рамці телефона.

## Як опублікувати

1. **GitHub:** створи новий репозиторій → *Add file → Upload files* → перетягни вміст цієї папки (index.html, assets, manifest.webmanifest, sw.js, README.md) → *Commit changes*.
2. **Vercel:** vercel.com → *Add New → Project* → *Import* свій репозиторій → Framework Preset: **Other** → *Deploy*. Налаштування збірки не потрібні.

Кожен новий коміт у GitHub автоматично оновлює сайт на Vercel.

Локально можна просто відкрити `index.html` у браузері.
