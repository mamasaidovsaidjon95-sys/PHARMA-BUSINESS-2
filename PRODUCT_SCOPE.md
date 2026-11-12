# Pharma Business — mahsulot doirasi

## Maqsad
Dorixona kundalik operatsiyalarini tartibli yuritish: mahsulot katalogi, partiya bo‘yicha ombor, kirim-chiqim, savdo va hisobotlar.

## Rollar (backend bosqichida)
- Egasi: barcha filiallar va sozlamalar.
- Administrator: katalog, ombor, foydalanuvchilar va hisobotlar.
- Farmatsevt: mahsulot qidirish, savdo va qaytarish.
- Kassir: savdo va chek.
- Kuzatuvchi: faqat o‘qish.

## Funksional talablar
1. Dori kartochkasi: nomi, SKU/shtrix-kod, kategoriya, ishlab chiqaruvchi, shakl, doza, birlik, kirim/sotuv narxi.
2. Partiya: seriya raqami, yaroqlilik muddati, miqdor, kirim narxi va yetkazib beruvchi.
3. Ombor: filial bo‘yicha qoldiq, minimal qoldiq, muddati yaqin/o‘tgan partiyalar.
4. Savdo: savatcha, chegirma, to‘lov turi, chek va sotuv tarixini yuritish.
5. Kirim: yetkazib beruvchi, hujjat raqami, partiya va narx.
6. Hamkorlar: mijozlar va yetkazib beruvchilar.
7. Hisobotlar: kunlik/oylik savdo, qoldiq, foyda (tannarx to‘liq yuritilgandan keyin), muddati yaqin mahsulotlar.
8. Xavfsizlik: autentifikatsiya, rollar, filialga tegishli ma’lumotni ajratish, audit log.
9. Zaxira: JSON/CSV eksport, keyinchalik avtomatik backup.

## Sifat va xavfsizlik
- Dori va partiya ma’lumotlari aniq saqlanishi kerak.
- Yaroqlilik muddati o‘tgan partiyalar savdoga berilmasligi kerak.
- Real dorixona ishga tushishidan oldin mahalliy qonunchilik, fiskal chek va ma’lumotlarni saqlash talablari tekshiriladi.
- Ilova klinik tashxis yoki dori buyurish vositasi emas.
