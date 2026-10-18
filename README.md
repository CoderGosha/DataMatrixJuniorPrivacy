# DataMatrixJuniorPrivacy

Статичные страницы Privacy Policy, Terms of Use и Support для приложения **DataMatrix Junior**, только на английском
(первая локаль приложения en-US). Подключён сабмодулем `Privacy/` в репозиторий приложения.

| Файл | Что это |
|---|---|
| `index.html` | Privacy Policy |
| `terms.html` | Terms of Use, в конце — лицензия zint (BSD-3 требует воспроизвести её в документации к приложению) |
| `support.html` | Support: частые вопросы и контакт |
| `style.css` | Цвета из `Common/Theme.swift` приложения, светлая и тёмная тема |
| `icon.svg` | Иконка приложения (Björk), копия `Design/AppIcon-Bjork.svg` |

Чистый HTML без сборки, ссылки относительные — как в `WeALocalPrivacy`.

Хостинг — GitHub Pages из ветки `main` (Settings → Pages → Deploy from a branch → `main` / root).

URL после включения Pages:

| Поле в App Store Connect | URL |
|---|---|
| Privacy Policy URL | `https://codergosha.github.io/DataMatrixJuniorPrivacy/` |
| Support URL | `https://codergosha.github.io/DataMatrixJuniorPrivacy/support.html` |
| License Agreement (если не стандартный EULA) | `https://codergosha.github.io/DataMatrixJuniorPrivacy/terms.html` |

## App Privacy в App Store Connect

По тому, что делает приложение сейчас, ответ — **Data Not Collected**: сети нет, аналитики и SDK нет, камера
и история сканов работают только на устройстве. Это совпадает с `PrivacyInfo.xcprivacy` приложения.

## Когда обновлять

При изменении того, как приложение обращается с данными, обновить текст и дату «Effective …» на обеих страницах.
Поводы, которые уже запланированы: печать на сетевые принтеры (раздел «Network printing» написан заранее),
iCloud-синхронизация Library, покупка Pro через StoreKit.
