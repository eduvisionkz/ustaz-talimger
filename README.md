# Ұстаз–тәлімгер

Ұстаздар күніне арналған сұхбат-жарияланым сайты: тәлімгер **Тогызбаева Айжан Хамзановна** мен жас маман **Қанапиянова Айзада Оралбекқызы** (Ш. Уәлиханов атындағы орта мектебі).

## Құрамы

```
ustaz-talimger/
├── index.html                  # сайттың өзі (HTML + CSS + JS бір файлда)
├── images/                     # оңтайландырылған фотолар
│   ├── hero.jpg  mentor_work.jpg  lesson.jpg
│   └── seminar.jpg  ai_event.jpg  classroom.jpg
├── .github/workflows/pages.yml # GitHub Pages-ке автоматты жариялау
├── .nojekyll
└── README.md
```

## GitHub Pages-ке жариялау (5 минут)

1. GitHub-та жаңа репозиторий ашыңыз (мысалы, `ustaz-talimger`), **Public**.
2. **Add file → Upload files** — осы архивтің ішіндегі барлық файл мен папканы сүйреп салыңыз (`.github` папкасымен бірге) → **Commit changes**.
3. **Settings → Pages → Build and deployment → Source: GitHub Actions** таңдаңыз.
4. **Actions** бөлімінде жариялау аяқталғанын күтіңіз (1–2 мин).
5. Сайт мекенжайы: `https://<логиніңіз>.github.io/ustaz-talimger/`

> `.github` папкасы жүктелмесе (кейбір браузерлер жасырын папканы өткізіп жібереді): **Settings → Pages → Source: Deploy from a branch → `main` / `(root)`** таңдаңыз — сайт workflow-сыз да жұмыс істейді.

### Git арқылы

```bash
git init
git add .
git commit -m "Ұстаз–тәлімгер сайты"
git branch -M main
git remote add origin https://github.com/<логин>/ustaz-talimger.git
git push -u origin main
```

## Өңдеу

- Мәтін — `index.html` ішінде, әр бөлім `<section id="...">` белгісімен.
- Фотоны ауыстыру — `images/` ішіндегі файлды сол атаумен алмастырыңыз.
- Түстер — `index.html` басындағы `:root { --navy, --gold, ... }` айнымалылары.

## Мүмкіндіктер

Мобильді құрылғыға бейімделген · жабысқақ мәзір белсенді бөлімді көрсетеді · сұхбат ашылмалы блоктар · фотогалерея (толық экран, ← → пернелері) · айналдыру анимациясы · басып шығаруға арналған стиль.
