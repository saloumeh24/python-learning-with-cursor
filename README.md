# python-learning-with-cursor
# تمرین‌های پایتون من

این مخزن شامل تمرین‌هایی است که در حال یادگیری پایتون انجام می‌دهم.

## برنامه‌های موجود

### 1. برنامه تشخیص سن (age_category.py)
این برنامه:
- از کاربر سن را می‌پرسد
- بر اساس سن، دسته سنی را مشخص می‌کند:
  - زیر 5 سال: کودک
  - بین 5 تا 13 سال: نوجوان
  - بالای 13 سال: بزرگسال

## چیزهایی که یاد گرفته‌ام
- کار با شرط‌ها (if/elif/else)
- گرفتن ورودی از کاربر
- تبدیل متن به عدد
===========================================================================
name = input("enter your name: ")
age = int(input("enter your age: "))
if age >= 18:
    message = f"welcome {name}"
else:
    message = f"sorry {name}, you are too young!"
print(message)
========================================================================
price = float(input("enter product price: "))
discount_percent = float(input("enter discount percentage: "))
discount_amount = price * (discount_percent / 100)
final_price = price - discount_amount

# روش مدرن با f-string
print(f"Original price: ${price:.2f}")
print(f"Discount amount: ${discount_amount:.2f}")
print(f"Final price: ${final_price:.2f}")
======================================================================================
age = 25
has_id = True

# استفاده از and
if age >= 18 and has_id:
    print("Can enter the club")

# استفاده از or
is_student = True
is_senior = False
if is_student or is_senior:
    print("Discount available")

# استفاده از not
is_closed = False
if not is_closed:
    print("Store is open")
==================================================================================================================
price = float(input("enter product price: "))
discount_percent = float(input("enter discount percentage: "))
discount_amount = price * (discount_percent / 100)
final_price = price - discount_amount

# روش مدرن با f-string
print(f"Original price: ${price:.2f}")
print(f"Discount amount: ${discount_amount:.2f}")
print(f"Final price: ${final_price:.2f}")

number = 10.3456
-------------------------
print(f"{number}")      # خروجی: 10.3456
print(f"{number:.2f}")  # خروجی: 10.35
print(f"{number:.1f}")  # خروجی: 10.3
print(f"{number:.3f}")  # خروجی: 10.346
--------------------
price = 49.9999
# روش‌های مختلف نمایش
print(f"قیمت: {price}")         # خروجی: 49.9999
print(f"قیمت: {price:.2f}")     # خروجی: 50.00
print(f"قیمت: ${price:.2f}")    # خروجی: $50.00
=================================================================================================================
# دریافت نمره از کاربر
score = float(input("Enter your score (0-100): "))

# دریافت وضعیت حضور
attendance = input("Did you attend the class? (yes/no): ")

# بررسی شرایط قبولی با استفاده از and
if score >= 60 and attendance.lower() == "yes":
    print(f"Your score is {score} and you attended the class - Pass")
else:
    print(f"Your score is {score} and your attendance is {attendance} - Fail")

--------------------------
attendance = input("Did you attend the class? (yes/no): ")

# فرض کنید کاربر "YES" وارد کرده
if attendance.lower() == "yes":    # "YES" تبدیل میشه به "yes"
    print("Condition met!")

# بدون lower() این مقایسه درست کار نمی‌کرد
if attendance == "yes":    # "YES" با "yes" برابر نیست!
    print("This might not work as expected!")
--------------------------------
# برنامه‌ای که پاسخ بله رو به هر شکلی قبول می‌کنه
answer = input("Are you ready? (yes/no): ")

if answer.lower() == "yes":
    print("Let's go!")
else:
    print("Take your time!")

# این برنامه همه این حالت‌ها رو "بله" در نظر می‌گیره:
# - "YES"
# - "Yes"
# - "yes"
# - "yEs"
# - "YeS"
=============================================================================================================
