<h1 align="center" style="font-size: 2.5em; margin-bottom: 15px; color: #2c3e50;">🚀 UTunnel Manager - راهکار حرفه‌ای تونلینگ امن</h1>

<h3 align="center" style="font-size: 1.4em; background: linear-gradient(90deg, #ff4d4d, #f9cb28); -webkit-background-clip: text; -webkit-text-fill-color: transparent; margin-bottom: 25px; padding: 10px; border-radius: 5px; border-left: 4px solid #e74c3c; border-right: 4px solid #e74c3c;">
🔥 عملکرد بی‌نظیر حتی روی سرورهای خارج از کشور با محدودیت شدید 🔥
</h3>


برای استفاده از تانل نیاز به ثبت آی پی دارید.

برای ثبت آی پی به ربات زیر بروید
https://t.me/utunnelipidf_bot
<div align="center" style="margin-bottom: 30px;">
  <img src="https://img.shields.io/badge/Go-1.21+-blue?style=for-the-badge&logo=go" alt="نسخه Go">
  <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge&logo=opensourceinitiative" alt="مجوز">
  <img src="https://img.shields.io/badge/Foreign_Servers-Supported-orange?style=for-the-badge&logo=serverless" alt="پشتیبانی از سرورهای خارج">
  
  <!-- دکمه‌های معماری‌های پشتیبانی شده -->
  <div style="margin-top: 15px;">
    <img src="https://img.shields.io/badge/x86_64-Supported-success?style=flat-square&logo=amd" alt="x86_64">
    <img src="https://img.shields.io/badge/ARM64-Supported-success?style=flat-square&logo=arm" alt="ARM64">
    <img src="https://img.shields.io/badge/RISC_V-Experimental-yellow?style=flat-square&logo=riscv" alt="RISC-V">
  </div>
</div>
 🌐 معرفی جامع
 
یک راهکار حرفه‌ای برای ایجاد تونل‌های امن و پرسرعت معکوس بین سرورهاست که با بهره‌گیری از آخرین فناوری‌های شبکه، امکان انتقال ترافیک با کمترین تاخیر را فراهم می‌کند. این سیستم به‌طور خاص برای محیط‌های حساس به تاخیر و نیازمند امنیت بالا طراحی شده است.

### 🔬 مشخصات فنی کلیدی

- **تاخیر**: <10ms در شبکه‌های بهینه‌شده
- 
- **پهنای باند**: پشتیبانی از Jumbo Frames (9000 بایت)
- 
- **امنیت**: TLS 1.3 با رمزنگاری AES-256-GCM
- 
- **بهینه‌سازی**: کاهش 40% مصرف CPU با الگوریتم‌های اختصاصی




## 🌟 پروتکل‌های کامل و کاربردهای آنها

| پروتکل       | 📌 ویژگی‌های کلیدی                        | 🏆 بهترین موارد استفاده      | 🔧 پارامترهای بهینه |
|--------------|------------------------------------------|-----------------------------|-------------------|
| **🛰️ TCP**      | 🔗 اتصال پایدار و مطمئن<br>📦 تضمین تحویل بسته‌ها<br>⚖️ کنترل جریان خودکار | 🖥️ انتقال فایل‌ها<br>📧 پروتکل‌های ایمیل<br>🌐 مرورگرهای وب | `window_size=256k`<br>`keepalive=60s` |
| **🌀 UDP**      | ⚡ سرعت بالا<br>🔄 ارتباط بدون اتصال<br>📡 مناسب برای داده‌های بلادرنگ | 🎮 بازی‌های آنلاین<br>📞 VoIP<br>📹 استریم ویدیو | `buffer=2MB`<br>`timeout=3s` |
| **🌐 WS**       | 🔄 ارتباط دوطرفه<br>🌍 مبتنی بر HTTP<br>🚀 مناسب برای وب‌سوکت‌ها | 💬 چت‌های بلادرنگ<br>📊 آپدیت‌های لحظه‌ای<br>🎮 بازی‌های مرورگری | `ping_interval=25s`<br>`max_size=1MB` |
| **🌉 TCPMux**   | 🔗 چندگانگی اتصالات<br>⚡ کاهش سربار<br>📦 بهینه برای داده‌های حجیم | 🖥️ انتقال داده‌های حجیم<br>🏢 ارتباطات سازمانی | `mux_con=8`<br>`timeout=30s` |
| **🕸️ WSMux**    | 🌐 ترکیب WebSocket + Muxing<br>🛡️ عبور از فایروال‌ها<br>🗜️ فشرده‌سازی | 💻 برنامه‌های وب پیشرفته<br>📱 ارتباطات موبایل | `compression=zlib`<br>`ping_interval=25s` |
| **🔐 WSS**      | 🔒 WS + SSL/TLS<br>🛡️ رمزنگاری end-to-end<br>📈 امنیت بالا | 🏦 تراکنش‌های مالی<br>🔐 لاگین‌های امن<br>🏥 داده‌های پزشکی | `tls_version=1.3`<br>`cert_check=strict` |
| **🔐 WSSMux**   | 🔒 WSMux + SSL/TLS<br>🛡️ امنیت end-to-end<br>📈 بهینه برای تراکنش‌ها | 🏦 سیستم‌های مالی<br> 🏥 ارتباطات پزشکی | `tls_version=1.3`<br>`cert_check=strict` |
| **🚄 UTCPmux**  | ⚡ بهینه‌سازی شده برای سرعت بالا<br>📡 Jumbo Frames<br>🌐 کاهش 40% CPU | 🖥️ مراکز داده<br>☁️ سرویس‌های ابری | `frame_size=9000`<br>`concurrency=16` |
| **🛡️ UWSmux**   | 🗜️ فشرده‌سازی هوشمند<br>⏱️ کاهش 30% تاخیر<br>🔄 بازیابی خودکار | 💼 ارتباطات سازمانی<br>🌍 سرویس‌های بین‌المللی | `compress_level=6`<br>`recovery_time=5s` |

## 📊 ماتریس انتخاب پروتکل - راهنمای جامع

این جدول به شما کمک می‌کند بر اساس نیازهای خود بهترین پروتکل را انتخاب کنید:

<div align="center">

| معیار        | توضیحات فنی                     | TCP  | TCPMux | UDP  | WS   | WSS  | WSMux | WSSMux | UTCPmux | UWSmux |
|--------------|----------------------------------|------|--------|------|------|------|-------|--------|---------|--------|
| **سرعت**     | میزان انتقال داده در ثانیه       | 🟢   | 🔵     | 🔵   | 🟢   | 🟡   | 🟢    | 🟡     | 🔵      | 🟢     |
| **امنیت**    | سطح رمزنگاری و حفاظت            | 🟡   | 🟡     | 🔴   | 🟡   | 🟢   | 🟡    | 🟢     | 🟢      | 🟢     |
| **پایداری**  | مقاومت در برابر قطع ارتباط     | 🟢   | 🟢     | 🔴   | 🟢   | 🟢   | 🟢    | 🟢     | 🔵      | 🟢     |
| **تاخیر**    | زمان پاسخگویی (میلی‌ثانیه)      | 🟡   | 🟡     | 🟢   | 🟡   | 🟡   | 🟡    | 🟡     | 🟢      | 🟢     |
| **بهینه‌سازی**| مصرف منابع سیستم               | 🟡   | 🟢     | 🟢   | 🟡   | 🟡   | 🟢    | 🟢     | 🟢      | 🟢     |

</div>

### 🧩 راهنمای انتخاب:
- **برای بازی‌های آنلاین**: UDP (تاخیر کم)
- **برای بانک‌داری**: WSSMux (امنیت بالا)
- **برای انتقال فایل‌های حجیم**: TCPMux (بهینه‌سازی منابع)
- **برای استریم ویدیو**: UTCPmux (پهنای باند بالا)
- **برای چت‌های سازمانی**: UWSmux (تعادل سرعت و امنیت)


### راهنما:
- 🟢 عالی
- 🔵 بسیار خوب
- 🟡 متوسط
- 🔴 پایه

### ✨ راهنمای انتخاب پروتکل:
1. **پایستگی**: 🛰️ TCP / 🌉 TCPMux
2. **سرعت**: 🌀 UDP 
3. **وب ساده**: 🌐 WS
4. **وب امن**: 🔐 WSS
5. **وب پیشرفته**: 🕸️ WSMux / 🔐 WSSMux
6. **بهینه‌سازی**: 🚄 UTCPmux (سرعت) / 🛡️ UWSmux (امنیت)

### ⚠️ نکات فنی:
- همیشه برای وب از نسخه‌های امن استفاده کنید
- تنظیمات `buffer` را با توجه به پهنای باند تنظیم نمایید
- برای برنامه‌های وب مدرن از WSMux استفاده کنید
- نسخه‌های **Mux** برای کاهش تاخیر و مصرف منابع مناسب‌اند

<div align="center"> <img src="https://github.com/user-attachments/assets/5a5792c8-b101-45fc-8843-6dd419fc8f33" alt="معماری سیستم" width="800"> <p><em>نمایی از معماری پیشرفته سیستم</em></p> </div>


⚙️ تنظیمات بهینه

✅ بهترین روش‌ها

برای ارتباطات وب: استفاده از UWSmux با تنظیمات پیش‌فرض

برای انتقال داده حجیم: UTCPmux با mux_version=2

تنظیمات امنیتی: فعال‌سازی TLS و استفاده از گواهی‌های معتبر

⚠️ نکات فنی مهم

همیشه از آخرین نسخه پروتکل استفاده کنید

برای تغییر نسخه، تمام پارامترهای مرتبط را بازتنظیم نمایید

از channel_size مناسب برای بار ترافیکی خود استفاده کنید

✅ همیشه از mux_version=2 استفاده کنید:

کاهش ۳۰-۵۰% نیاز به mux_con

بهبود ۲۰-۴۰% عملکرد کلی

مصرف منابع کمتر

⚠️ تذکر مهم: هنگام تغییر نسخه، حتما channel_size و connection_pool را نیز تنظیم مجدد کنید!

🖼️ گالری تصاویر 

<div align="center"> <table> <tr> <td><img src="https://github.com/user-attachments/assets/09f19faa-d157-40d6-a7d1-0e4d31607297" width="400" alt="نمونه 1"></td> <td><img src="https://github.com/user-attachments/assets/9ae26d5a-b008-4543-8156-1f8afbcad86f" width="400" alt="نمونه 2"></td> <td><img src="https://github.com/user-attachments/assets/395ff89e-bef0-4cbc-bec5-70e501171761" width="400" alt="نمونه 4"></td> </tr> </table> </div>
📝 راهنمای جامع حالت‌های عملیاتی

🔵 حالت سرور (اجرا روی سرور ایران)

نام سرویس: هر نامی با حروف و اعداد انگلیسی (منحصر به فرد در هر سرور)

توکن: باید مطابق با مقدار سرور خارج باشد

پورت تانل: باید با مقدار سرور خارج یکسان باشد

mux_con: تعداد کانکشن‌های مولتی‌پلکس (پیش‌فرض: 8)

🟢 حالت کلاینت (اجرا روی سرور خارج)

نیاز به آیپی سرور ایران و پورت تانل (مطابق با تنظیمات سرور)

🟡 سایر حالت‌ها:

وضعیت: نمایش وضعیت تانل‌ها

ریستارت: راه‌اندازی مجدد یک یا همه تانل‌ها

توقف: متوقف کردن یک یا همه سرویس‌های تانل

حذف: حذف یک یا همه تانل‌ها

تایمر: تنظیم ریستارت خودکار (1 تا 23 ساعت)

🔧 نمونه‌های تنظیمات پورت
```
443-600                  # گوش دادن به پورت‌های 443-600 و فوروارد به همان پورت‌ها در مقصد
443-600:5201             # گوش دادن به 443-600 و فوروارد به پورت 5201
443-600=1.1.1.1:5201     # گوش دادن به 443-600 و فوروارد به پورت 5201 روی IP 1.1.1.1
443                      # گوش دادن به پورت 443 و فوروارد به پورت 443 مقصد
4000=5000                # گوش دادن به 4000 و فوروارد به 5000
127.0.0.2:443=5201       # گوش دادن به 443 روی IP 127.0.0.2 و فوروارد به 5201
443=1.1.1.1:5201         # گوش دادن به 443 و فوروارد به 5201 روی 1.1.1.1
127.0.0.2:443=1.1.1.1:5201  # گوش دادن به 443 روی 127.0.0.2 و فوروارد به 5201 روی 1.1.1.1
```
💻 راهنمای نصب و اجرا

برای پردازنده‌های x86/x64 (AMD64):

```
wget https://raw.githubusercontent.com/aliamg1356/utunnel/refs/heads/main/utunnel_manager_amd64
chmod +x utunnel_manager_amd64
./utunnel_manager_amd64
```
برای پردازنده‌های ARM64:

```
wget https://raw.githubusercontent.com/aliamg1356/utunnel/refs/heads/main/utunnel_manager_arm64
chmod +x utunnel_manager_arm64
./utunnel_manager_arm64
```
برای پردازنده‌های x86 (32 بیتی):

```
wget https://raw.githubusercontent.com/aliamg1356/utunnel/refs/heads/main/utunnel_manager_386
chmod +x utunnel_manager_386
./utunnel_manager_386
```
🤖 نصب ربات تلگرام مونیتورینگ

```
bash <(curl -s https://raw.githubusercontent.com/aliamg1356/utunnel/refs/heads/main/MonitorBotinstall.sh --ipv4)
```
پس از اجرا:

گزینه نصب را انتخاب کنید

توکن ربات و چت آی دی خود را وارد نمایید

زمان بررسی تانل‌ها را بر اساس ثانیه تنظیم کنید

## 💰 حمایت مالی

به علت عدم حمایت مالی از انتشار عمومی تانل به صورت رایگان منصرف شدم



<div align="center"> <table> <tr> <td><img src="https://github.com/user-attachments/assets/29063460-b7f5-4e59-88df-bbe4bb84c836" width="300"></td> <td><img src="https://github.com/user-attachments/assets/c2f33b82-46ad-46c8-b514-2d017532e5f4" width="300"></td> </tr> <tr> <td><img src="https://github.com/user-attachments/assets/e7fbaa6e-2d6a-48c8-9696-0cc8ab528a14" width="300"></td> <td><img src="https://github.com/user-attachments/assets/59322989-d5ae-472f-a491-34104ec85b74" width="300"></td> </tr> </table> </div>
