# 🎼 Nota Pleyeri

Brauzerda ishlaydigan nota (MusicXML) pleyeri: VexFlow bilan nota ko'rinishi, Tone.js bilan ijro, real vaqtda nota yoritilishi.

## Imkoniyatlar
- MusicXML / JSON yuklash (drag-and-drop)
- Dinamika (pp–ff, crescendo/decrescendo), staccato, accent, fermata
- BPM slayderi, cholg'u tanlash (fortepiano, skripka, fleyta), Humanize
- Chalinayotgan notani highlight qilish

## Ishga tushirish
`index.html` ni brauzerda oching, yoki GitHub Pages orqali joylang:
1. Repo → **Settings → Pages**
2. Source: **Deploy from a branch** → `main` / `(root)`
3. Saqlang, bir necha daqiqadan keyin sayt tayyor bo'ladi.

## PDF / rasm (OMR)
PDF va rasm skaneri uchun alohida backend (FastAPI + Audiveris) kerak. `index.html` ichidagi `OMR_URL` o'zgaruvchisini backend manzilingizga o'zgartiring. Backend `POST /omr` qabul qilib, MusicXML matnini qaytarishi kerak.

## Soundfont
Haqiqiy cholg'u namunalari uchun `makeInstrument()` ichiga `soundfont-player` ulash mumkin (lokal yoki GitHub Pages'da ishlaydi).

## Litsenziya
MIT
