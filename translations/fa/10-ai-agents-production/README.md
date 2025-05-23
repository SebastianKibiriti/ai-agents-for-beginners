<!--
CO_OP_TRANSLATOR_METADATA:
{
  "original_hash": "44013a98d980c8b92d4b814dc49b545d",
  "translation_date": "2025-03-28T09:45:21+00:00",
  "source_file": "10-ai-agents-production\\README.md",
  "language_code": "fa"
}
-->
[![AI Agents In Production](../../../translated_images/lesson-10-thumbnail.0b68f4240618b3d5b26693b78cf2cf0a8b36131b50bb08daf91d548cecc87424.fa.png)](https://youtu.be/l4TP6IyJxmQ?si=IvCW3cbw0NJ2mUMV)

> _(برای مشاهده ویدئوی این درس، تصویر بالا را کلیک کنید)_
# عوامل هوش مصنوعی در محیط تولید

## مقدمه

در این درس به موارد زیر پرداخته می‌شود:

- نحوه برنامه‌ریزی برای استقرار مؤثر عامل هوش مصنوعی در محیط تولید.
- اشتباهات و مشکلات رایج که ممکن است هنگام استقرار عامل هوش مصنوعی در محیط تولید با آن‌ها مواجه شوید.
- نحوه مدیریت هزینه‌ها در عین حفظ عملکرد عامل هوش مصنوعی.

## اهداف یادگیری

پس از تکمیل این درس، خواهید دانست که چگونه:

- تکنیک‌هایی برای بهبود عملکرد، هزینه‌ها و اثربخشی یک سیستم عامل هوش مصنوعی در محیط تولید.
- چه چیزی و چگونه عوامل هوش مصنوعی خود را ارزیابی کنید.
- چگونه هزینه‌ها را هنگام استقرار عوامل هوش مصنوعی در محیط تولید کنترل کنید.

استقرار عوامل هوش مصنوعی قابل اعتماد اهمیت زیادی دارد. درس "ساخت عوامل هوش مصنوعی قابل اعتماد" را نیز بررسی کنید.

## ارزیابی عوامل هوش مصنوعی

قبل، حین و بعد از استقرار عوامل هوش مصنوعی، داشتن یک سیستم مناسب برای ارزیابی آن‌ها بسیار حیاتی است. این کار اطمینان می‌دهد که سیستم شما با اهداف شما و کاربران هماهنگ است.

برای ارزیابی یک عامل هوش مصنوعی، مهم است که بتوانید نه تنها خروجی عامل، بلکه کل سیستمی که عامل در آن فعالیت می‌کند را ارزیابی کنید. این شامل موارد زیر می‌شود، اما محدود به آن‌ها نیست:

- درخواست اولیه مدل.
- توانایی عامل در شناسایی هدف کاربر.
- توانایی عامل در شناسایی ابزار مناسب برای انجام وظیفه.
- پاسخ ابزار به درخواست عامل.
- توانایی عامل در تفسیر پاسخ ابزار.
- بازخورد کاربر نسبت به پاسخ عامل.

این فرآیند به شما امکان می‌دهد تا نقاط ضعف را به صورت ماژولار شناسایی کنید. سپس می‌توانید تأثیر تغییرات مدل‌ها، درخواست‌ها، ابزارها و سایر مؤلفه‌ها را با کارایی بیشتر نظارت کنید.

## مشکلات رایج و راه‌حل‌های ممکن در عوامل هوش مصنوعی

| **مشکل**                                      | **راه‌حل ممکن**                                                                                                                                                                                                     |
| ---------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| عامل هوش مصنوعی وظایف را به طور منظم انجام نمی‌دهد | - درخواست داده شده به عامل هوش مصنوعی را اصلاح کنید؛ اهداف را به وضوح مشخص کنید.<br>- بررسی کنید که آیا تقسیم وظایف به وظایف کوچکتر و مدیریت آن‌ها توسط عوامل متعدد کمک می‌کند.                                                      |
| عامل هوش مصنوعی وارد حلقه‌های پیوسته می‌شود         | - شرایط و ضوابط پایان فرآیند را به وضوح تعریف کنید تا عامل بداند چه زمانی باید متوقف شود.<br>- برای وظایف پیچیده که نیاز به استدلال و برنامه‌ریزی دارند، از مدل بزرگتری که برای وظایف استدلال تخصصی است استفاده کنید. |
| درخواست‌های ابزار عامل هوش مصنوعی عملکرد خوبی ندارند | - خروجی ابزار را خارج از سیستم عامل آزمایش و اعتبارسنجی کنید.<br>- پارامترهای تعریف شده، درخواست‌ها و نام‌گذاری ابزارها را اصلاح کنید.                                                                                        |
| سیستم چند عامله عملکرد ثابتی ندارد               | - درخواست‌های داده شده به هر عامل را اصلاح کنید تا اطمینان حاصل شود که مشخص و متمایز از یکدیگر هستند.<br>- یک سیستم سلسله‌مراتبی با استفاده از عامل "مسیر‌یابی" یا کنترل‌کننده ایجاد کنید تا تعیین کند کدام عامل مناسب است.         |

## مدیریت هزینه‌ها

در اینجا برخی استراتژی‌ها برای مدیریت هزینه‌های استقرار عوامل هوش مصنوعی در محیط تولید آورده شده است:

- **ذخیره‌سازی پاسخ‌ها** - شناسایی درخواست‌ها و وظایف رایج و ارائه پاسخ‌ها قبل از عبور آن‌ها از سیستم عامل، روش خوبی برای کاهش حجم درخواست‌های مشابه است. حتی می‌توانید یک جریان برای شناسایی میزان شباهت درخواست با درخواست‌های ذخیره شده خود با استفاده از مدل‌های هوش مصنوعی ساده‌تر اجرا کنید.

- **استفاده از مدل‌های کوچک‌تر** - مدل‌های زبان کوچک (SLMs) می‌توانند در برخی موارد استفاده عامل، عملکرد خوبی داشته باشند و هزینه‌ها را به طور قابل توجهی کاهش دهند. همان‌طور که قبلاً ذکر شد، ایجاد یک سیستم ارزیابی برای تعیین و مقایسه عملکرد در مقابل مدل‌های بزرگ‌تر بهترین راه برای درک عملکرد یک SLM در مورد استفاده شما است.

- **استفاده از مدل مسیریاب** - یک استراتژی مشابه استفاده از تنوع مدل‌ها و اندازه‌ها است. می‌توانید از یک LLM/SLM یا تابع بدون سرور برای مسیریابی درخواست‌ها بر اساس پیچیدگی به مدل‌های مناسب استفاده کنید. این کار همچنین به کاهش هزینه‌ها کمک می‌کند و عملکرد در وظایف مناسب را تضمین می‌کند.

## تبریک

این درس فعلاً آخرین درس "عوامل هوش مصنوعی برای مبتدیان" است.

ما قصد داریم بر اساس بازخورد و تغییرات در این صنعت در حال رشد، درس‌های بیشتری اضافه کنیم، بنابراین در آینده نزدیک دوباره مراجعه کنید.

اگر می‌خواهید یادگیری و ساخت با عوامل هوش مصنوعی را ادامه دهید، به <a href="https://discord.gg/kzRShWzttr" target="_blank">دیجورد انجمن Azure AI</a> بپیوندید.

ما در آنجا کارگاه‌ها، میزگردهای جامعه و جلسات "هر چه می‌خواهید بپرسید" برگزار می‌کنیم.

ما همچنین مجموعه‌ای از مطالب آموزشی اضافی داریم که می‌تواند به شما کمک کند تا شروع به ساخت عوامل هوش مصنوعی در محیط تولید کنید.

## درس قبلی

[الگوی طراحی فراشناخت](../09-metacognition/README.md)

**سلب مسئولیت**:  
این سند با استفاده از سرویس ترجمه هوش مصنوعی [Co-op Translator](https://github.com/Azure/co-op-translator) ترجمه شده است. در حالی که ما تلاش می‌کنیم دقت را حفظ کنیم، لطفاً توجه داشته باشید که ترجمه‌های خودکار ممکن است شامل خطاها یا نادقتی‌ها باشند. سند اصلی به زبان اصلی آن باید به عنوان منبع معتبر در نظر گرفته شود. برای اطلاعات حساس، توصیه می‌شود از ترجمه حرفه‌ای انسانی استفاده شود. ما مسئولیتی در قبال سوءتفاهم‌ها یا تفسیرهای نادرست ناشی از استفاده از این ترجمه نداریم.