# DMD Mebel paneli — ish holati

Yangi chatga shu fayl bilan o'tiladi.

## Tuzilishi
- **Panel:** `index.html` (bitta fayl, repo ildizida) → GitHub `main` → Vercel.
- **Server:** `DMD-Sotuv.gs` — alohida (standalone) Apps Script loyihasi. **Repoga qo'yilmaydi**, chatda beriladi, deployni egasi qiladi.
- **Jadval:** «DMD мебкл продажа» — `База` va `План` varaqlari. Faqat o'qiladi. Jadval ichidagi egasining o'z skriptiga («DMD» menyusi) tegilmaydi.

## Chap panel
| Bo'lim | Holati |
|---|---|
| Бошқарув панели | ishlaydi (sotuv ma'lumotidan) |
| Сотув | ishlaydi: Умумий · Масъуллар · Маҳсулотлар · План · Сотувлар |
| Маркетинг | тез орада |
| Молия | тез орада |
| Склад | тез орада |

## Ma'lumot qoidalari
- `База`: Дата · Магазин · Ответственный · Продукт · Тип · Тип число · Число · Цена. Bitta qator = bitta sotuv.
- Tushum = «Цена» yig'indisi («Цена» — sotuvning umumiy summasi, dona narxi emas).
- Miqdor («Число») birligi bo'yicha alohida sanaladi: шт va кв qo'shilmaydi.
- `План`: oyma-oy bloklar (sana → Продукт | План | Факт | Колди). Plan varaqdan olinadi, **fakt esa `База`dan hisoblanadi** (o'sha oy, mahsulot nomi bo'yicha). Varaqdagi «Факт» bilan farq bo'lsa panel ogohlantiradi.
- Pul birligi: `$` (`index.html` → `PUL_OLDI`). Tasdiqlanishi kerak.

## Havolalar va versiyalar
- `API_SOTUV` (`index.html`): ulangan (2026-10-10). Jonli javob hali tekshirilmagan.
- `DMD-Sotuv.gs`: v1.0

## Keyingi qadamlar
1. Jonli ma'lumotni brauzerda tekshirish (`/exec?amal=tekshir`, `sinov()` natijasi).
3. Маркетинг / Молия / Склад jadvallari tayyor bo'lganda ulash.
4. Kerak bo'lsa — PIN bilan kirish (hozircha o'chiq).
