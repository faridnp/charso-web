# Charso Web

وب‌سایت بازی چهارسو. فایل‌های قابل انتشار داخل پوشه `www/` قرار دارند.

## استقرار روی up.platenumber9.ir

با هر push به شاخه `main`، محتویات `www/` از طریق FTP به مسیر `public_html/up/` روی هاست ارسال می‌شوند. این مسیر باید در cPanel به‌عنوان Document Root زیردامنه `up.platenumber9.ir` تنظیم شده باشد (مسیر کامل هاست: `/home/platen/public_html/up/`).

در مخزن GitHub از مسیر **Settings → Secrets and variables → Actions** این سه Secret را بسازید: `FTP_SERVER`، `FTP_USERNAME` و `FTP_PASSWORD`. هیچ رمز یا توکنی را داخل فایل‌ها یا گفتگو قرار ندهید.

**هشدار استقرار:** این مقصد، ریشه سایت `up.platenumber9.ir` است؛ فایل‌های سایت قبلی در همین پوشه ممکن است با استقرار چهارسو جایگزین یا همگام‌سازی شوند. قبل از اولین Deploy مطمئن شوید که قصد دارید چهارسو روی ریشه همین زیردامنه قرار بگیرد.
