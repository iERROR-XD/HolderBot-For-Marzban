![Example Image](holderbotcover.png)


# هولدربات چیه؟ (ورژن 3.2.1)
هولدر بات یه ربات سریع و ساده‌ست که برای حل مشکل عدم وجود گزینه `شروع تایمر پس از اولین اتصال` در رابط کاربری "پنل مرزبان" ساخته شده. با استفاده از رابط‌های برنامه نویسی `پنل مرزبان`، هولدر بات بهت این امکان رو می‌ده که به راحتی از این قابلیت در تلگرام استفاده کنید. ولی بعد از آپدیت 3.0 هولدربات قضیه یکمی متفاوت تر شد و هولدربات امکانات خاصی برای کاربران عرضه کرد. برای اطلاعات بیشتر به قسمت بروزرسانی ها مراجعه کنید و یا در کانال [@ErfjabHolderbot](https://t.me/ErfjabHolderbot) عضو شوید ، نصب کنید و لذت ببرید.

# چجوری نصب کنیم؟ (همچنین آپدیت)
برای آپدیت ابتدا توکن بات را revoke کنید. سپس برای نصب فقط کافیه دستورات زیر را در سرور ابونتوی خود وارد کنید.
```
cd && cd .. && rm install.sh*
```

```
sudo apt install && sudo apt-get install libjpeg-dev && wget https://raw.githubusercontent.com/iERROR-XD/HolderBot-For-Marzban
/main/install.sh && chmod +x install.sh && ./install.sh
```
حالا که همه پیش‌نیازها نصب شدن، برای استارت زدن ربات اطلاعات زیر رو بهش بدید.

</details>

<details  markdown="1"> <summary>در صورت نیاز به حذف کامل بات کلیک کنید.</summary>

```
if ps aux | grep -v grep | grep "python3 holderbot.py" &> /dev/null; then
    echo "Stopping existing holderbot process..."
    pkill -f "python3 holderbot.py"
fi

if ps aux | grep -v grep | grep "python3 node_status_checker.py" &> /dev/null; then
    echo "Stopping existing holderbot process..."
    pkill -f "python3 node_status_checker.py"
fi

if ps aux | grep -v grep | grep "python3 holder.py" &> /dev/null; then
    echo "Stopping existing holder process..."
    pkill -f "python3 holder.py"
fi

if [ -d "holder" ]; then
    echo "Directory holder already exists. Deleting..."
    rm -rf holder
fi
```

</details>

| اطلاعات | توضیحات |
| --- | --- |
| شناسه کاربری ادمین | شناسه کاربری تلگرامی شخصی که می‌خواهد از ربات استفاده کند. می‌توانید این اطلاعات را از این ربات بدست آورید. [@userinfobot](https://t.me/userinfobot) |
| توکن ربات تلگرام | توکن بات تلگرامی خود را میتوانید از طریق [@BotFather](https://t.me/botfather) بدست آورید. |
| نام کاربری پنل | می‌توانید نام کاربری مدیر اصلی را وارد کنید. |
| رمز عبور پنل | می‌توانید رمز عبور مدیر اصلی را وارد کنید. |
| دامنه پنل | ساب دامنه پنل خود را وارد کنید، بدون 'https://' ولی با پورت ، مانند: sub.domain.com:port |

اگر اطلاعاتتون رو به درستی وارد کرده باشید، یک پیامی به این شکل دریافت خواهید کرد.

![Example Image](nohupshot.png)

**صفحه را همانطور که هست نگه دارید و اکنون ربات را تست کنید. اگر اطلاعات شما صحیح باشد، ربات برای شما کاربر ایجاد می کند و اگر صحیح نباشد، کاربر ایجاد نمی کند.**
اگر ربات برای شما کاربر ایجاد نکرد، به صفحه بازگردید و دستور زیر را اجرا کنید.
```
Ctrl C
```
سپس دوباره از ابتدا مراحل نصب را طی کنید، فقط در تکمیل اطلاعات خود دقت کنید.

**اکنون، اگر این بار کاربر ربات ساخته است، پس لذت ببرید.** (سرور رو بدون دستوری ببندید.)

# بروزرسانی و امکانات جدید ؟

<details  markdown="1"> <summary>نسخه‌ی 1.0</summary>

  - تولد هولدربات و امکان دریافت ساخت یوزر با قابلیت شروع تایم بعد اولین اتصال. 

</details>

<details  markdown="1"> <summary>نسخه‌ی 2.0</summary>

  - امکان ساخت دسته جمعی یوزر. 

</details>

<details  markdown="1"> <summary>نسخه‌ی 3.0</summary>

  - امکان مانیتورینگ لحظه ای نود ها
  - ارسال نوتیف هنگام قطع شدن نودها
  - امکان انتخاب اینباند‌ هنگام ساخت یوزر
  - امکان دریافت آمار کلی کاربران پنل تعداد و لیست‌شون 
  - (مخصوصا کاربران آنلاین و آفلاین در 24 ساعت اخیر)
  - امکان دریافت آمار تکی کاربر با اسم یا لینک ساب 
  - (مخصوصا آخرین تایم آپدیت ساب و آنلاینی)
  - امکان دریافت آمار با لینک ساب توسط کاربر از بات
  - رفع باگ اذیت کننده‌ی credentials
</details>


آپدیت 4.0؟ بعد 150 ستار‌ه شدن گیت‌هاب! برای `بورزسانی و افزودن امکانات جدید` به بات ، میتوانید به گیت هاب هولدربات ستاره بدید. برای هرگونه سوال ، گزارش باگ و پیشنهادات میتوانید ایشو کنید. ممنونیم 🫶🏻

# چجوری استفاده کنیم؟ 

چنل [@ErfjabHolderbot](https://t.me/ErfjabHolderbot) جهت ارائه آموزش ها ، اطلاع رسانی های آپدیت ها ، نظرسنجی ها برای اضافه شدن ویژگی های جدید و از این قبیل تشکیل شده است.

<p align="center">
  <a target="_blank" href="https://t.me/ErfjabHolderbot">
    <img alt="Telegram Badge" src="https://img.shields.io/badge/holderbotchanel-Telegramlink?style=for-the-badge&logo=telegram&logoColor=white&color=blue&link=https%3A%2F%2Ft.me%2FErfjabHolderbot&link=https%3A%2F%2Ft.me%2FErfjabHolderbot">
  </a>
</p>

