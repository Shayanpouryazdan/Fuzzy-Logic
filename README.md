

---

# 🔍 Fuzzy Logic System for Customer Loyalty Prediction

# 🔍 سیستم فازی برای پیش‌بینی وفاداری مشتری

---

## 🧠 Problem Statement | بیان مسئله

**EN:**
In the competitive world of e-commerce, retaining loyal customers is essential. Traditional methods often struggle with vague behavioral data. This project uses **fuzzy logic** to estimate a customer's loyalty based on monthly purchases, discount habits, membership duration, and inactivity days.

**FA:**
در دنیای رقابتی فروشگاه‌های اینترنتی، حفظ مشتریان وفادار نقش کلیدی در موفقیت دارد. روش‌های سنتی معمولاً در مواجهه با داده‌های رفتاری مبهم کارایی لازم را ندارند. این پروژه با استفاده از **منطق فازی**، میزان وفاداری مشتری را بر اساس میزان خرید ماهانه، نسبت خرید در زمان تخفیف، مدت عضویت و تعداد روزهای غیرفعال پیش‌بینی می‌کند.

---

## 🔧 How It Works | نحوه عملکرد

**EN:**

1. Inputs are fuzzified using membership functions.
2. Rules (if-then) are applied.
3. Results are aggregated and defuzzified using centroid method.
4. Final loyalty score (0–100) is produced.

**FA:**

1. مقادیر ورودی با استفاده از توابع عضویت فازی‌سازی می‌شوند.
2. قوانین فازی «اگر–آنگاه» اعمال می‌شوند.
3. خروجی قوانین تجمیع و سپس با روش مرکز ثقل غیرفازی‌سازی می‌شود.
4. در نهایت، یک مقدار بین ۰ تا ۱۰۰ به‌عنوان امتیاز وفاداری مشتری به دست می‌آید.

---

## 🎯 Inputs & Output | ورودی‌ها و خروجی

* `monthly_purchase` → میزان خرید ماهانه (۱ تا ۲۰ میلیون تومان)
* `discount_ratio` → درصد خرید در زمان تخفیف (۰ تا ۱۰۰)
* `membership_duration` → مدت عضویت (۰ تا ۶۰ ماه)
* `inactive_days` → تعداد روزهای غیرفعال بودن مشتری در ماه (۰ تا ۳۰)
* **Output:** میزان وفاداری مشتری (۰ تا ۱۰۰)

---

## 📝 Example | مثال اجرا

```python
# Example input
loyalty_sim.input['monthly_purchase'] = 12     # million Toman
loyalty_sim.input['discount_ratio'] = 40       # %
loyalty_sim.input['membership_duration'] = 24  # months
loyalty_sim.input['inactive_days'] = 10        # days

# Compute
loyalty_sim.compute()
print(f"Loyalty Score: {loyalty_sim.output['loyalty']:.2f} / 100")
```

---

## 📁 Files | فایل‌ها

* `loyalty_system.py` → کد اصلی سیستم فازی
* `example.ipynb` → مثال اجرایی با جداول و نمودار
* `rules_table.pdf` → جدول قوانین فازی
* `README.md` → مستندات پروژه

---

## 🚀 Advantages | مزایا

| روش                        | مزایا                                   |
| -------------------------- | --------------------------------------- |
| Fuzzy Logic                | تفسیر پذیر، مناسب برای داده‌های نامطمئن |
| Machine Learning           | دقت بالا، قابل یادگیری خودکار           |
| Purchase Behavior Analysis | مبتنی بر رفتار واقعی مشتری، قابل تعمیم  |

---

## 📊 Future Plans | توسعه‌های آتی

* اتصال به پایگاه داده واقعی فروشگاه
* افزودن الگوریتم یادگیری قوانین فازی
* طراحی داشبورد بصری برای تحلیل بازاریابی

---

## 📄 License | مجوز

MIT License – استفاده آزاد با حفظ حقوق نویسنده.

---

