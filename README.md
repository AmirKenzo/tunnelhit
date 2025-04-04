✨ پروژه پیشرفته UTunnel Manager ✨
<div align="center"> <img src="https://img.shields.io/badge/Go-1.21+-blue?style=for-the-badge" alt="نسخه Go"> <img src="https://img.shields.io/badge/License-MIT-green?style=for-the-badge" alt="مجوز"> <img src="https://img.shields.io/badge/Supports-ARM64%20%26%20x86-brightgreen?style=for-the-badge" alt="پشتیبانی معماری"> <img src="https://img.shields.io/badge/Version-2.0.0-red?style=for-the-badge" alt="نسخه"> </div>

 🌐 معرفی جامع
UTunnel Manager یک راهکار حرفه‌ای برای ایجاد تونل‌های امن و پرسرعت بین سرورهاست که با بهره‌گیری از آخرین فناوری‌های شبکه، امکان انتقال ترافیک با کمترین تاخیر را فراهم می‌کند. این سیستم به‌طور خاص برای محیط‌های حساس به تاخیر و نیازمند امنیت بالا طراحی شده است.

🔍 ویژگی‌های کلیدی
انتقال ترافیک با تاخیر کمتر از 10ms در شبکه‌های بهینه

مصرف منابع سیستم بهینه‌شده

پشتیبانی از آخرین استانداردهای امنیتی

مدیریت هوشمند پهنای باند


🛡️ پروتکل‌های پشتیبانی شده

🔹 پروتکل‌های پایه

TCP: پایدار و قابل اعتماد

UDP: مناسب برای ارتباطات بلادرنگ

پروتکل‌های پیشرفته:

TCPMux

WS (WebSocket)

WSS (WebSocket Secure با SSL)

WSMux

WSSMux

UTCPmux (نسخه بهینه‌شده)

UWSmux (نسخه پیشرفته)


🌟 ویژگی‌های منحصر به فرد

تولید خودکار گواهی SSL سلف‌ساین برای رمزگذاری ارتباطات

پشتیبانی از پروتکل‌های اختصاصی با عملکرد فوق‌العاده:

🚄 UTCPmux (بهینه‌شده)

کاهش 40% مصرف CPU نسبت به نسخه استاندارد

پشتیبانی از Jumbo Frames برای شبکه‌های پرسرعت

بهبود پایداری ارتباط

🌐 UWSmux (پیشرفته)

قابلیت فشرده‌سازی داده‌ها

کاهش 30% تاخیر ارتباطات

مکانیزم بازیابی خودکار هنگام قطعی

بهترین انتخاب برای ارتباطات امن وب‌محور


<div align="center"> <img src="https://github.com/user-attachments/assets/5a5792c8-b101-45fc-8843-6dd419fc8f33" alt="نمونه اولیه" width="700"> </div>
🛠️ تنظیمات بهینه

✅ UWSmux: بهترین انتخاب برای ارتباطات امن وب‌محور با تأخیر کم

✅ UTCPmux: راهکار ایده‌آل برای انتقال‌های پرحجم در شبکه‌های پرسرعت

✅ همیشه از mux_version=2 استفاده کنید:

کاهش ۳۰-۵۰% نیاز به mux_con

بهبود ۲۰-۴۰% عملکرد کلی

مصرف منابع کمتر

⚠️ تذکر مهم: هنگام تغییر نسخه، حتما channel_size و connection_pool را نیز تنظیم مجدد کنید!

🖼️ گالری تصاویر 

<div align="center"> <table> <tr> <td><img src="https://github.com/user-attachments/assets/09f19faa-d157-40d6-a7d1-0e4d31607297" width="400" alt="نمونه 1"></td> <td><img src="https://github.com/user-attachments/assets/9ae26d5a-b008-4543-8156-1f8afbcad86f" width="400" alt="نمونه 2"></td> </tr> <tr> <td><img src="https://github.com/user-attachments/assets/019d6d11-c264-4a0a-b1d7-b25dc03d6396" width="400" alt="نمونه 3"></td> <td><img src="https://github.com/user-attachments/assets/395ff89e-bef0-4cbc-bec5-70e501171761" width="400" alt="نمونه 4"></td> </tr> </table> </div>
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

💰 حمایت مالی


اگر تمایل به حمایت مالی از توسعه این پروژه دارید، می‌توانید از طریق آدرس‌های کیف پول زیر اقدام نمایید:

<div align="center">
	آدرس کیف پول
 
  
Tron Network	TRX	TMXRpCsbz8PKzqN4koXiErawdLXzeinWbQ

Ethereum	USDT (ERC20)	0xD4cEBA0cFf6769Fb9EFE4606bE59C363Ff85BF76

</div><div align="center" style="margin-top: 20px;"> <p>🙏 از حمایت شما سپاسگزاریم. هر مقدار کمک مالی به توسعه و بهبود مستمر پروژه کمک می‌کند.</p> </div>
🖼️ تصاویر اضافی

<div align="center"> <table> <tr> <td><img src="https://github.com/user-attachments/assets/29063460-b7f5-4e59-88df-bbe4bb84c836" width="300"></td> <td><img src="https://github.com/user-attachments/assets/c2f33b82-46ad-46c8-b514-2d017532e5f4" width="300"></td> </tr> <tr> <td><img src="https://github.com/user-attachments/assets/e7fbaa6e-2d6a-48c8-9696-0cc8ab528a14" width="300"></td> <td><img src="https://github.com/user-attachments/assets/59322989-d5ae-472f-a491-34104ec85b74" width="300"></td> </tr> </table> </div>
