# Ma’lumotlar modeli

Asosiy bog‘lanishlar:
- `pharmacies` — biznes/dorixona tashkiloti.
- `pharmacy_members` — foydalanuvchi va uning roli.
- `branches` — filiallar.
- `medicines` — mahsulot katalogi.
- `stock_batches` — partiya, seriya va yaroqlilik muddati bo‘yicha qoldiq.
- `suppliers`, `customers` — kontragentlar.
- `purchase_receipts` — kirim hujjatlari.
- `sales`, `sale_items` — savdo sarlavhasi va tarkibi.
- `stock_movements` — ombor harakatlarining auditga yaroqli jurnali.
- `audit_log` — muhim amallar tarixi.

Savdo paytida partiya qoldig‘i tranzaksiya ichida kamaytirilishi, muddati o‘tgan partiyalar bloklanishi va tegishli `stock_movements` yozuvi yaratilishi kerak. Buni production backend'da server-side SQL function yoki API orqali amalga oshiring.
