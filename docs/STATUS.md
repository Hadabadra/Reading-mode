# היכן אוחזים – מצב קריאה

**גרסה אחרונה:** 2.1.0 (04.11.2026) – Release ‏v2.1.0 עם `reading-mode-2.1.0.otzplugin`.

## פרסום לחנות – פתוח
ה-workflow ‏`.github/workflows/store.yml` עובר ולידציה (0 שגיאות) ויוצר Release, **אבל לא מפרסם לחנות**: בריפו הזה אין סודות `OTZARIA_USER` / `OTZARIA_PASSWORD` (בלוג ה-action לא מופיעים `otzaria-user`/`otzaria-password`). סשן של Claude לא יכול להגדיר סודות.
לביצוע: Settings ← Secrets and variables ← Actions ← להוסיף את שני הסודות (אותם ערכים כמו ב-KLI-MULON) ← Actions ← "פרסום לחנות אוצריא" ← Run workflow. לחלופין להעלות ידנית את קובץ ה-otzplugin מה-Release.

## בוצע ב-2.1.0
כל 7 ההערות מקובץ ההערות של 04.11 (ראו CHANGELOG בתוך התוסף ו-`docs/default-text-reader.md`).

## רעיונות פתוחים (לא בוצעו)
- אין API להכניס מספרי עמודים לחלונית הניווט של אוצריא – יש ניווט משלנו (Ctrl+G, מספרים בתוכן העניינים של לשונית התוסף).
- "מעבר לקורא רגיל" בתפריט "עוד" הוא של אוצריא – לא ניתן להסתיר.
- הערות עיצוב של המאמת (px, צבעי hex, font-family של David בייצוא) – לא חוסמות; לטיפול אם רוצים את תג "מראה תואם".
- `events.subscribe:theme.changed` ו-`app.info.read` ניתנות כיום אוטומטית – אפשר להסיר מהמניפסט (לא נגעתי בהרשאות).
