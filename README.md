# Charso Web

وب‌سایت بازی چهارسو. فایل‌های قابل انتشار داخل پوشه `www/` قرار دارند.

## استقرار روی up.platenumber9.ir

با هر push به شاخه `main`، محتویات `www/` از طریق GitHub Actions و FTP به مسیر `public_html/up/` ارسال می‌شوند. مسیر کامل مورد انتظار روی هاست: `/home/platen/public_html/up/`؛ این مسیر باید Document Root زیردامنه `up.platenumber9.ir` باشد.

در مخزن GitHub از مسیر **Settings → Secrets and variables → Actions** این سه Secret را اضافه کنید: `FTP_SERVER`، `FTP_USERNAME` و `FTP_PASSWORD`. اطلاعات ورود FTP را در کد یا گفتگو قرار ندهید.

پس از اضافه کردن سایت به مخزن و ثبت Secretها، هر push به `main` اجرا شدن گردش Deploy را آغاز می‌کند.
