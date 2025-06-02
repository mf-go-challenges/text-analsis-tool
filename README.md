# text-analsis-tool
Write a program that reads text files and gives simple information about their content. The program should do these things:

1. Read all text files in a folder.
2. Count and show:

   * How many times each word appears.
   * The average length of words.
   * Which words appear most often.
   * How many sentences there are.
   * How many paragraphs there are.

**The program should also:**

* Be able to read text from different sources:

  * From files on your computer,
  * From text you type in the command line,
  * Or from a web address (URL).
* Let you save results in different formats:

  * JSON (a common text format),
  * CSV (a simple table format),
  * Or plain text.
* Work on more than one file at the same time (parallel processing).
* Handle errors when reading or writing files. For example, if a file is missing, show a clear error message.
* Let the user choose options when they start the program (using command-line arguments). For example, the user can say which folder to use or which output format to save.
* Save the final results to new files, using different naming rules (for example, adding “\_stats” to the file name).

**To build this program, you will need to:**

* Organize your code into different parts (for example, one part for reading files, one part for calculating statistics, one part for writing results).
* Write functions that can read and write data in different ways.
* Open and read files, and then close them correctly.
* Count words and calculate averages.
* Keep track of words and their counts (for example, using a map or dictionary).
* Handle mistakes or problems (for example, a file does not exist).
* Run several tasks at the same time to make the program faster (parallel processing).
* Let the user pass options when they run the program (command-line arguments).
* Create the output in a clear format (JSON, CSV, or plain text).

**A simple project structure could be:**

```
textAnalyzer/
├── main.go          
├── analyzer/        
│   └── analyzer.go   (code to calculate statistics)
├── iomanager/       
│   └── iomanager.go  (code to read and write files)
├── statistics/      
│   └── statistics.go (more code for finding word counts, averages)
├── output/          
│   └── output.go     (code to create JSON, CSV, or text files)
└── config/          
    └── config.go     (code to read command-line options)
```

This project is similar in difficulty to a simple calculator you might build, but now you will learn how to work with files, count words, and run tasks in parallel.

---

# **نسخهٔ فارسی**

یک برنامه بنویسید که فایل‌های متنی را می‌خواند و اطلاعات ساده‌ای دربارهٔ محتوای آن‌ها می‌دهد. برنامه باید این کارها را انجام دهد:

1. همهٔ فایل‌های متنی را در یک پوشه بخواند.
2. بشمرد و نشان دهد:

   * هر کلمه چند بار تکرار شده است.
   * طول متوسط کلمات چقدر است.
   * کدام کلمات بیشترین تکرار را دارند.
   * چند جمله وجود دارد.
   * چند پاراگراف وجود دارد.

**همچنین برنامه باید:**

* بتواند متن را از منابع مختلف بخواند:

  * از فایل‌های کامپیوتر،
  * از متنی که در خط فرمان تایپ می‌کنید،
  * یا از یک آدرس اینترنتی (URL).
* به شما اجازه دهد نتایج را با فرمت‌های مختلف ذخیره کنید:

  * JSON (یک فرمت متنی رایج)،
  * CSV (یک فرمت سادهٔ جدولی)،
  * یا متن ساده.
* روی بیش از یک فایل به صورت همزمان کار کند (پردازش موازی).
* در حین خواندن یا نوشتن فایل‌ها خطاها را مدیریت کند. مثلاً اگر یک فایل وجود ندارد، پیام خطای واضحی نمایش دهد.
* به کاربر اجازه دهد گزینه‌ها را هنگام اجرای برنامه انتخاب کند (استفاده از آرگومان‌های خط فرمان). برای مثال، کاربر می‌تواند پوشهٔ ورودی یا فرمت خروجی را مشخص کند.
* نتایج نهایی را در فایل‌های جدید ذخیره کند و از قوانین نام‌گذاری مختلف استفاده کند (مثلاً اضافه کردن “\_stats” به نام فایل).

**برای ساخت این برنامه، باید:**

* کد خود را به بخش‌های مختلف تقسیم کنید (مثلاً یک بخش برای خواندن فایل‌ها، یک بخش برای محاسبهٔ آمار، یک بخش برای نوشتن نتایج).
* توابعی بنویسید که بتوانند داده‌ها را به روش‌های مختلف بخوانند و بنویسند.
* فایل‌ها را باز و خوانده و سپس ببندید.
* کلمات را بشمارید و میانگین طول آن‌ها را محاسبه کنید.
* تعداد کلمات و تکرار هر کلمه را ذخیره کنید (برای مثال با استفاده از یک ساختار شبیه دیکشنری).
* خطاها یا مشکلات را مدیریت کنید (مثلاً اگر فایل وجود ندارد).
* چندین کار را به طور همزمان اجرا کنید تا برنامه سریع‌تر شود (پردازش موازی).
* به کاربر اجازه دهید هنگام اجرای برنامه از طریق خط فرمان، گزینه‌هایی را وارد کند.
* خروجی را در فرمت‌های واضح و خوانا ایجاد کنید (JSON، CSV یا متن ساده).

**ساختار سادهٔ پروژه می‌تواند به صورت زیر باشد:**

```
textAnalyzer/
├── main.go          
├── analyzer/        
│   └── analyzer.go   (کدی برای محاسبهٔ آمار)
├── iomanager/       
│   └── iomanager.go  (کدی برای خواندن و نوشتن فایل‌ها)
├── statistics/      
│   └── statistics.go (کد بیشتر برای شمارش کلمات و محاسبهٔ میانگین)
├── output/          
│   └── output.go     (کدی برای تولید فایل‌های JSON، CSV یا متن)
└── config/          
    └── config.go     (کدی برای خواندن گزینه‌های خط فرمان)
```

این پروژه از نظر سختی شبیه یک ماشین‌حساب ساده است که ممکن است قبلاً ساخته باشید، اما این بار شما با فایل‌ها کار می‌کنید، کلمات را می‌شمارید و پردازش موازی را یاد می‌گیرید.

## The project structure could look like:
```
textAnalyzer/
├── main.go
├── analyzer/
│   └── analyzer.go
├── iomanager/
│   └── iomanager.go
├── statistics/
│   └── statistics.go
├── output/
│   └── output.go
└── config/
    └── config.go
```

This challenge maintains the same level of complexity and learning opportunities as your price calculator project but focuses on a different domain. It would help you practice the same Go concepts while working on a new and interesting problem.