# Joylashtirish

## GitHub Pages (faqat statik demo)
1. Repository root'iga `index.html`, `src/`, `public/` va boshqa fayllarni yuklang.
2. GitHub → Settings → Pages.
3. Source: Deploy from a branch.
4. Branch: `main`; folder: `/(root)`; Save.
5. Sayt URL'i GitHub Pages sahifasida ko‘rinadi.

## Backend haqida
GitHub Pages faqat statik frontendni host qiladi. Login, umumiy baza va telefonlararo sinxronlash uchun alohida backend kerak (masalan, Supabase yoki boshqa server). `migrations/001_initial_schema.sql` — boshlang‘ich PostgreSQL sxemasi, to‘liq tayyor production backend emas.

## Xavfsizlik
- API secret/service-role key'larni HTML yoki JS ichiga yozmang.
- RLS siyosatlarini tekshirmasdan real mijoz yoki savdo ma’lumotlarini kiritmang.
- Ishga tushirishdan oldin backup/restore jarayonini sinang.
