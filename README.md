# feedback-board
Simple feedback management system with Flask, SQLite, Bootstrap, and Docker. Users submit feedback; admin changes the status (registered/reviewed/handled)

## تصمیمات فنی
به طور خلاصه اگر بخوام بگم
- خب برای پیاده سازیش پایتون رو انتخاب کردم به دلیل اینکه هم تجربه کدنویسی با این زبان رو داشتم هم خیلی راحت میشد باهاش یک API
رو پیاده سازی کرد

- API : خب چون پروژه ساده هست و نیازی به (API) سنگین و پیچیده نیست برای همین از Flask استفاده کردم

- Database :
-  خب برای دیتابیس هم شما اختیار استفاده از دیتابیس های مختلف رو داده بودین
هر چند میشد با SQLAlchemy هم دیتابیس رو پیاده سازی کرد ولی بنظرم چون کوئری های ساده ای تسک داشت و نیازی به استفاده از دیتابیس های پیچیده تر نبود و همچنین با توجه به پروژه ای که خودم این ترم دارم کوئری های ساده رو با Sqlite طراحی کنی واقعا بهتر از دیتابیس های سنگین جواب میده و سریع تره

- Frontend :
-  خب برای فرانت هم از HTML , Bootstrap استفاده کردم
خب شما گفته بودین که صرفا ساخت سریع یک ظاهر تمیز و قابل استفاده کفایت میکنه
و نیازی به طراحی یک سایت با ظاهر کاملا متفاوت و خاص نداشت
و خب Bootstrap هم کامپوننت های آماده داشتم منم ازش استفاده کردم

## نحوه اجرا (لوکال)

- کلون کردن مخزن:
```bash
git clone https://github.com/MortezaMotahar/feedback-board.git
cd feedback-board
python -m venv venv
pip install -r requirements.txt
echo "SECRET_KEY=test123" > .env   # یک کلید خودتون بهش بدید
python app.py
```
- یا اینکه فایل هارو دانلود کرده و در ابتدا فایل پایتون را ران کنید و سپس با آدرس های لوکال هاست به صفحه های مورد نظر بروید


## نصاویر
<img width="1920" height="1024" alt="ثبت فیدبک" src="https://github.com/user-attachments/assets/869e79df-a0f6-4f6b-b0d9-35aa047d3024" />
<img width="1917" height="1026" alt="لاگین ادمین" src="https://github.com/user-attachments/assets/fb56b16a-c744-4393-85c4-120142bcd0ac" />
<img width="1915" height="1028" alt="لیست فیدبک ها" src="https://github.com/user-attachments/assets/ef690f95-bba1-4082-9ae5-936527d4e3a2" />


همچنین دیپلوی شده روی آدرس : https://BlackHole.pythonanywhere.com/

- درمورد فایل Docker صادقانه باید بگم که داکر رو من بیشتر از یک سال قبل محتوایی رو درموردش دیدم و الان حضور ذهن زیادی ندارم ، صرفا از یک سری اطلاعات کمم توانستم قسمت هایی رو پیاده سازی کنم برای همین مطمئن نیستم فایل داکری که ساختم درست باشد یا نه
