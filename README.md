# PHARMA BUSINESS
**Dorixona boshqaruvi uchun web-ilova — GitHub repository paketi**

> Ushbu paket Pharma Business loyihasining boshlang‘ich GitHub versiyasidir. Unda dorilar katalogi, partiya va yaroqlilik muddati, savdo savatchasi, kirim, kontragentlar, hisobotlar va sozlamalar uchun ishlaydigan demo interfeys bor. Hozirgi demo ma’lumotlarni shu brauzer qurilmasidagi `localStorage` ichida saqlaydi.

## Asosiy modullar
- Dashboard: savdo, mahsulotlar, qoldiq va muddati yaqin partiyalar ko‘rsatkichlari.
- Dorilar: nomi, kodi, kategoriya, sotib olish/sotish narxi va minimal qoldiq.
- Ombor: partiyalar, miqdor, yaroqlilik muddati va partiya bo‘yicha qoldiq.
- Savdo: savatcha, miqdor, chegirma, jami va chekni chop etish.
- Kirim: yetkazib beruvchidan mahsulot qabul qilish.
- Yetkazib beruvchilar va mijozlar ro‘yxati.
- Hisobot: savdo yozuvlari va CSV eksport.
- Sozlamalar: dorixona nomi, valyuta va ogohlantirish chegarasi.

## Ishga tushirish
Bu versiya statik web-ilova:
1. ZIP faylni oching.
2. `index.html` faylini brauzerda oching yoki GitHub repository root'iga yuklang.
3. GitHub Pages kerak bo‘lsa: **Settings → Pages → Deploy from a branch → main → /(root) → Save**.
4. Ilovani `https://<username>.github.io/<repository>/` manzilida oching.

## Muhim cheklovlar
- Bu build **demo/MVP**: ma’lumotlar bitta brauzer qurilmasida saqlanadi; telefonlar o‘rtasida avtomatik sinxronlash yo‘q.
- Hozircha login, rollar bo‘yicha server tekshiruvi, real to‘lov, fiskal kassa integratsiyasi, E-IMZO yoki davlat tizimlari bilan aloqa yo‘q.
- `migrations/001_initial_schema.sql` Supabase/PostgreSQL uchun keyingi backend bosqichining boshlang‘ich sxemasidir. Uni production bazaga qo‘llashdan oldin administrator/DB mutaxassisi tekshirishi kerak.
- Ilova dori tanlash yoki davolash bo‘yicha klinik tavsiya bermaydi. Dorilarni sotish va hisobini yuritish uchun mo‘ljallangan.

## Papkalar
```text
PHARMA-BUSINESS/
├── index.html
├── README.md
├── .gitignore
├── public/
│   └── favicon.svg
├── src/
│   ├── app.js
│   └── styles.css
├── migrations/
│   └── 001_initial_schema.sql
└── docs/
    ├── PRODUCT_SCOPE.md
    ├── DATA_MODEL.md
    └── DEPLOYMENT.md
```

## Keyingi ishlab chiqish bosqichlari
1. Supabase loyihasi va xavfsiz server-side autentifikatsiya.
2. RLS siyosatlari va foydalanuvchi rollari (egasi, administrator, farmatsevt, kassir).
3. Bir nechta filial va filiallararo ombor harakati.
4. Audit log, zaxira nusxa va ma’lumotlarni eksport/import qilish.
5. Chek printeri va qonuniy talab qilinadigan fiskal tizimlar bilan integratsiya.
6. iPhone/Android PWA sinovi va qurilmalararo sinxronlash.

## GitHub'ga yuklash
Repository nomi: `PHARMA-BUSINESS`. ZIP ichidagi fayllarni repository root'iga joylang (ZIP faylning o‘zini emas, ichidagi papka va fayllarni yuklang). `README.md` avtomatik ko‘rinadi.
