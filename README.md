# 🕌 سلاطین دکن هند (۱۵۰۰–۱۷۰۰) | نسخه تعاملی و ترجمه فارسی
### Sultans of Deccan India, 1500–1700: Opulence and Fantasy

[![Live Demo](https://img.shields.io/badge/Live_Site-GitHub_Pages-brightgreen?style=for-the-badge&logo=github)](https://dalroot.github.io/sultans-deccan-persian/)
[![Academic Translation](https://img.shields.io/badge/Translation-Ph.D._Thesis-blue?style=for-the-badge)](#شناسنامه-علمی-و-دست‌اندرکاران)
[![ORCID](https://img.shields.io/badge/ORCID-0009--0005--6825--6728-a6ce39?style=for-the-badge&logo=orcid&logoColor=white)](https://orcid.org/0009-0005-6825-6728)
[![Open Access](https://img.shields.io/badge/Access-Open_Academic-orange?style=for-the-badge)](#مجوز-و-حقوق-معنوی)

<p align="center">
  <img src="og_preview.jpg" alt="پیش‌نمایش سلاطین دکن هند" width="850" style="border-radius: 12px; box-shadow: 0 10px 30px rgba(0,0,0,0.5);">
</p>

---

## 📖 درباره پروژه (About The Project)

این مخزن شامل **ترجمه کامل فارسی، سیستم دیجیتال تعاملی و نسخه مدون چاپی** کتاب مرجع و تحسین‌شده **«سلاطین دکن هند (۱۵۰۰–۱۷۰۰): شکوه و خیال»** (*Sultans of Deccan India, 1500–1700: Opulence and Fantasy*) منتشر شده توسط **موزه هنر متروپولیتن نیویورک (The Metropolitan Museum of Art)** است.

فرهنگ و هنر پادشاهی‌های دکن (احمدنگر، بیجاپور، گلکنده، بیدر و برار) یکی از درخشان‌ترین و پیوندخورده‌ترین دوره‌های تاریخ هنر جهان اسلام با زبان، ادب و نگارگری ایرانی و هندی به شمار می‌آید. این پروژه، این اثر فاخر را به همراه تمام نگاره‌ها، اسناد تصویری و تحلیل‌های باستان‌شناختی و هنری در بستری مدرن، تعاملی و با دسترسی باز (Open Access) در اختیار پژوهشگران، دانشجویان و علاقه‌مندان فارسی‌زبان قرار می‌دهد.

* 🌐 **مشاهده آنلاین سامانه تعاملی:** [https://dalroot.github.io/sultans-deccan-persian/](https://dalroot.github.io/sultans-deccan-persian/)

---

## ✨ ویژگی‌های شاخص سامانه (Features)

- 📱 **خوانشگر وب کاملاً ریسپانسیو (Responsive Web Reader):** طراحی اختصاصی برای مطالعه بدون نقص در تمامی نمایشگرها (موبایل، تبلت و دسکتاپ).
- 📑 **بخش‌بندی مهندسی‌شده (Modular 10-Page Chunks):** تقسیم ۳۸۶ صفحه به بسته‌های خوانش ۱۰ صفحه‌ای برای بارگذاری سریع، خوانایی روان و بهینه‌سازی مصرف حافظه.
- 🎨 **گالری کامل مینیاتورها و آثار موزه‌ای:** شامل ۳۸۴ اثر هنری، مرقعات، نگاره‌های دربار دکن و نسخه‌های خطی همراه با زیرنویس‌های تحلیلی و تخصصی.
- 🔤 **تایپوگرافی آکادمیک فارسی:** استفاده از فونت استاندارد و چشم‌نواز **وزیرمتن (Vazirmatn)** با رعایت دقیق اصول چیدمان راست‌به‌چپ (RTL) و ارجاعات دوزبانه.
- 🖨️ **نسخه‌های جامع چاپی (Complete A4 PDFs):** نسخه‌های آماده چاپ با حروف‌چینی صفحه‌آرایی‌شده آکادمیک در پوشه `output_pdf/`.
- ⚙️ **خط لوله پردازش خودکار (Automated Pipeline):** مجهز به اسکریپت‌های پایتون جهت استخراج متن، تطبیق واژه‌نامه تخصصی اصطلاحات تاریخی/هنری (Glossary) و بیلد وب‌سایت.

---

## 🗂 ساختار مخزن (Repository Structure)

```plaintext
sultans-deccan-persian/
├── index.html                     # هاب اصلی داشبورد و فهرست تعاملی فصول
├── index_reader.html              # خوانشگر یکپارچه
├── Vazirmatn-Regular.ttf          # فونت بهینه شده وزیرمتن
├── Vazirmatn-Bold.ttf             # فونت بولد وزیرمتن
├── og_preview.jpg                 # تصویر پیش‌نمایش متادیتای شبکه‌های اجتماعی
├── responsive_chunks/             # بسته‌های ده‌صفحه‌ای تعاملی وب (صفحات ۱۱ تا ۳۸۶)
│   ├── pages_011_to_020_responsive.html
│   ├── pages_021_to_030_responsive.html
│   └── ...
├── output_pdf/                    # فایل‌های خروجی و نسخه‌های کامل
│   ├── Sultans_of_Deccan_India_Persian_Translation_Complete.pdf
│   ├── Sultans_of_Deccan_Persian_Thesis_Final.pdf
│   └── Sultans_of_Deccan_Persian_Complete.html
└── *.py                           # اسکریپت‌های پردازش متن، واژه‌نامه و ساخت صفحات
    ├── pipeline_step1_pdfplumber_extract.py
    ├── pipeline_step2_translate_pages.py
    ├── pipeline_step3_render_final_pdf.py
    ├── build_responsive_reader.py
    └── update_all_responsive_chunks.py
```

---

## 🚀 نحوه استفاده و اجرای محلی (Quick Start & Usage)

### ۱. دسترسی مستقیم (آنلاین)
بدون نیاز به نصب یا دانلود، مستقیماً از طریق نشانی زیر مطالعه کنید:
👉 **[https://dalroot.github.io/sultans-deccan-persian/](https://dalroot.github.io/sultans-deccan-persian/)**

### ۲. اجرای آفلاین و محلی (Local Hosting)
برای اجرای پروژه روی رایانه شخصی:

```bash
# ۱. کلون کردن مخزن
git clone https://github.com/dalroot/sultans-deccan-persian.git
cd sultans-deccan-persian

# ۲. اجرای سرور ساده وب (پایتون)
python3 -m http.server 8080
```
سپس در مرورگر خود نشانی `http://localhost:8080` را باز کنید.

---

## 🎓 شناسنامه علمی و دست‌اندرکاران (Academic Credits)

* **اثر مرجع:** *Sultans of Deccan India, 1500–1700: Opulence and Fantasy* (Navina Najat Haidar & Marika Sardar, The Metropolitan Museum of Art, New York).
* **ترجمه پایان‌نامه دکترا:** خانم **انوشه طاهری**
* **توسعه سامانه دیجیتال و ناظر فنی:** **توانا محمدی (Tawana Mohammadi)**
  * شناسه پژوهشی بین‌المللی: [![ORCID](https://img.shields.io/badge/ORCID-0009--0005--6825--6728-a6ce39?style=flat-square&logo=orcid&logoColor=white)](https://orcid.org/0009-0005-6825-6728)

---

## ⚖️ حقوق معنوی و استفاده آموزشی (Academic Disclaimer)

این پروژه با اهداف صرفاً **پژوهشی، علمی، دانشگاهی و غیرتجاری** آماده‌سازی شده است تا دسترسی جامعه علمی و فارسی‌زبانان به یکی از مهم‌ترین منابع تاریخ هنر دوره دکن و پیوندهای تمدنی ایران و هند را تسهیل نماید. کلیه حقوق مادی و معنوی اثر اصلی متعلق به **موزه هنر متروپولیتن نیویورک** و پدیدآورندگان اثر اصلی می‌باشد.
