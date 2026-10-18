# FigCraft فارسی

نسخهٔ فارسی و راست‌به‌چپ [FigCraft](https://github.com/storytold/figcraft): طراحی رابط، متن‌باز، نوشته‌شده با Rust.

این فورک روی حساب [Reza-Nozari](https://github.com/Reza-Nozari) است تا فارسی‌زبان‌ها ترجمه را بازبینی کنند، راست‌به‌چپ را بهتر کنند و Pull Request بفرستند. داستان بقیهٔ اپ‌ها: [artcraft-farsi](https://github.com/Reza-Nozari/artcraft-farsi).

راهنمای انگلیسی ساخت و معماری در [README.md](README.md) مانده است.

## الان چه هست

کار فارسی روی شاخهٔ [`persian`](https://github.com/Reza-Nozari/figcraft/tree/persian) است:

- زبان پیش‌فرض رابط، فارسی است.
- صفحهٔ خانه و پنل طراحی برای راست‌به‌چپ آینه می‌شوند.
- قلم‌های فارسی (مثل Vazirmatn و Tahoma) در فهرست جایگزین‌ها هستند.
- متن‌های رابط در [`crates/ui-egui/locales/fa.toml`](crates/ui-egui/locales/fa.toml) است. وضعیت این فایل پیش‌نویس است و به بازبینی یک فارسی‌زبان نیاز دارد.

شناسهٔ فرمان‌ها انگلیسی می‌ماند تا منو، خط فرمان و بقیهٔ ابزارها با هم بخوانند. فقط نوشته‌ای که کاربر می‌بیند ترجمه می‌شود.

## چطور کمک کنید

۱. مخزن [Reza-Nozari/figcraft](https://github.com/Reza-Nozari/figcraft) را فورک کنید.
۲. شاخهٔ `persian` را پایه بگیرید.
۳. ترجمه را در `crates/ui-egui/locales/fa.toml` اصلاح کنید، یا چیدمان راست‌به‌چپ را در رابط بهتر کنید.
۴. Pull Request را به شاخهٔ `persian` همین مخزن بفرستید، نه به storytold، مگر اینکه خودتان بخواهید تغییر را به پروژهٔ اصلی هم پیشنهاد دهید.

نام برندها و کلیدهای میانبر را دست نزنید. اگر جمله‌ای در فایل ترجمه نیست، رابط همان متن انگلیسی را نشان می‌دهد.

جزئیات روش ترجمه در `docs/translating.md` است.

## ساخت

همان روش پروژهٔ اصلی:

```bash
cargo run -p figcraft
```

بعد از ساخت، رابط باید فارسی و از راست به چپ باز شود.
