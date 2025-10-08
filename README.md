# triage

# عنوان: نقش هوش مصنوعی در تریاژ بیمارستانی (مرور کوتاه)

## 1. مقدمه
- تعریف تریاژ و اهمیت آن در ED.
- محدودیت‌های تریاژ انسانی: تغییرپذیری و خطای مistriage. (ارجاع به مرورها).  [oai_citation:16‡BioMed Central](https://bmcemergmed.biomedcentral.com/articles/10.1186/s12873-024-01135-2?utm_source=chatgpt.com)
- جملهٔ هدف: "هدف این مرور کوتاه بررسی روش‌های AI برای پشتیبانی از تریاژ ED، منابع دادهٔ عمومی، و خلأهای پژوهشی برای کار آینده است."

## 2. منابع دادهٔ عمومی و نقش آن‌ها
- MIMIC-IV: منبع اصلی و پرکاربرد برای مطالعاتED. (شرح مختصر + citation).  [oai_citation:17‡PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC9810617/?utm_source=chatgpt.com)
- MC-MED و MIMIC-IV-Ext: منابع چندوجهی و corpusهای تریاژ برای LLM.  [oai_citation:18‡PhysioNet](https://physionet.org/content/mc-med/?utm_source=chatgpt.com)

## 3. چه مدل‌هایی استفاده شده‌اند — دسته‌بندی بر اساس ورودی
- Vital-signs based models: LR, XGBoost (نمونه: Xie et al.).  [oai_citation:19‡arXiv](https://arxiv.org/pdf/2111.11017?utm_source=chatgpt.com)
- Text/NLP models: BERT/LLM برای chief complaint (مثال MIMIC-IV-Ext).  [oai_citation:20‡PhysioNet](https://physionet.org/content/?topic=emergency+triage&utm_source=chatgpt.com)
- Multimodal: ترکیب عددی+متن+waveforms (MC-MED).  [oai_citation:21‡PhysioNet](https://physionet.org/content/mc-med/?utm_source=chatgpt.com)

## 4. شواهد اثربخشی و محدودیت‌ها
- خلاصهٔ نتایج: مطالعات نشان می‌دهند ML می‌تواند دقت تریاژ را افزایش دهد اما اغلب فاقد اعتبارسنجی چندمرکزی و real-world deployment هستند.  [oai_citation:22‡BioMed Central](https://bmcemergmed.biomedcentral.com/articles/10.1186/s12873-024-01135-2?utm_source=chatgpt.com)
- چالش‌ها: explainability، bias، real-time inference، تنظیم رگولاتوری.

## 5. مسیر پیشنهادی ما (کار خودِ شما)
- پیشنهاد: توسعه یک مدل کمکی برای پیش‌بینی ESI (levels 1–5) با ورودی‌های vitals + short chief complaint، استفاده از MIMIC-IV (یا dataset محلی) برای آموزش و MC-MED برای اعتبارسنجی خارجی.  [oai_citation:23‡PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC9810617/?utm_source=chatgpt.com)
- نکات عملی: human-in-the-loop، شرح‌پذیری (SHAP), audit logging، IRB & data agreements.

## 6. جمع‌بندی
- AI پتانسیل دارد ولی نیاز به اعتبارسنجی و توجه به عدالت/شفافیت دارد.
- منابع کلیدی: (فهرست bib کوتاه: Johnson2023, Xie2021, Liu2021, MC-MED2025, MIMIC-IV-Ext2025,...).  [oai_citation:24‡PMC](https://pmc.ncbi.nlm.nih.gov/articles/PMC9810617/?utm_source=chatgpt.com)
