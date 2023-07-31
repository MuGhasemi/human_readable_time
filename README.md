# زمان خوانا

این یک تابع پایتون است که عددی غیر منفی (ثانیه) را به عنوان ورودی می‌گیرد و زمان را با فرمت خوانا (ساعت:دقیقه:ثانیه) برمی‌گرداند.

## چگونه استفاده کنیم

1. مخزن را در دستگاه محلی خود کلون کنید.
2. تابع `make_readable` را از ماژول `time_utils` وارد کنید.
3. تابع `make_readable` را فراخوانی کنید و تعداد ثانیه‌ها را به عنوان آرگومان ارسال کنید.

مثال:

```python
from time_utils import make_readable1 #OR make_readable2

seconds = 3661
result = make_readable1(seconds)
print(result)  # خروجی: 01:01:01
```

## جزئیات تابع

تابع `make_readable` ساعت، دقیقه و ثانیه را از تعداد داده شده ثانیه‌ها محاسبه کرده و آن‌ها را با رشته‌ی خوانا فرمت می‌کند. این تابع از تابع `divmod()` برای محاسبه کارآمد و f-string برای فرمت‌بندی خروجی با صفر اولیه استفاده می‌کند.

# Human Readable Time

This is a Python function that takes a non-negative integer representing the number of seconds and returns the time in a human-readable format (HH:MM:SS).

## How to Use

1. Clone the repository to your local machine.
2. Import the `make_readable` function from the `time_utils` module.
3. Call the `make_readable` function and pass the number of seconds as an argument.

Example:

```python
from time_utils import make_readable #OR make_readable2

seconds = 3661
result = make_readable1(seconds)
print(result)  # Output: 01:01:01
```

## Function Details

The `make_readable` function calculates the hours, minutes, and seconds from the given number of seconds and formats them in a human-readable string. It uses the `divmod()` function for efficient calculation and f-string for formatting the output with leading zeros.
