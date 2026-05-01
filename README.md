# 💱 Currency Converter Pro

<div align="center">
  <img src="icon2.png" width="120" alt="Currency Converter Pro"/>
  
  **محوّل العملات الاحترافي**
  
  [![Deploy to GitHub Pages](https://github.com/YOUR_USERNAME/currency-converter-pro/actions/workflows/deploy-pages.yml/badge.svg)](https://github.com/YOUR_USERNAME/currency-converter-pro/actions/workflows/deploy-pages.yml)
  [![Build APK](https://github.com/YOUR_USERNAME/currency-converter-pro/actions/workflows/build-apk.yml/badge.svg)](https://github.com/YOUR_USERNAME/currency-converter-pro/actions/workflows/build-apk.yml)
</div>

---

## ✨ المميزات

- 🌍 دعم **50+ عملة** عالمية
- 📊 **رسم بياني** تاريخي للأسعار
- 🌐 **3 لغات**: العربية، الإنجليزية، الفرنسية
- 📱 **PWA** – يعمل بدون إنترنت
- ⚡ تحديث تلقائي كل 5 ثوانٍ
- 🎨 واجهة احترافية داكنة

---

## 🗂️ هيكل الملفات

```
currency-converter-pro/
├── index.html          ← الصفحة الرئيسية
├── manifest.json       ← إعدادات PWA
├── sw.js               ← Service Worker (الوضع دون إنترنت)
├── icon2.png           ← أيقونة التطبيق
└── .github/
    └── workflows/
        ├── deploy-pages.yml  ← نشر GitHub Pages
        └── build-apk.yml     ← بناء APK
```

---

## 🚀 خطوات النشر على GitHub والحصول على APK

### الخطوة 1: رفع المشروع على GitHub

```bash
git init
git add .
git commit -m "🚀 Initial commit - Currency Converter Pro"
git remote add origin https://github.com/USERNAME/currency-converter-pro.git
git push -u origin main
```

### الخطوة 2: تفعيل GitHub Pages

1. اذهب إلى **Settings** في مستودعك
2. اختر **Pages** من القائمة الجانبية
3. في **Source** اختر **GitHub Actions**
4. انتظر دقيقة وسيكون التطبيق متاحاً على:
   `https://USERNAME.github.io/currency-converter-pro/`

### الخطوة 3: الحصول على APK عبر PWABuilder (الأسهل ✅)

1. افتح الموقع: **https://www.pwabuilder.com**
2. أدخل رابط GitHub Pages الخاص بك
3. اضغط **Start** ثم اختر **Android**
4. اضغط **Generate Package**
5. حمّل ملف APK وثبّته على هاتفك!

### الخطوة 4 (اختياري): بناء APK تلقائياً عبر GitHub Actions

أضف هذه الـ **Secrets** في إعدادات GitHub:
- `KEYSTORE_BASE64` → ملف keystore بصيغة base64
- `KEY_ALIAS` → اسم الـ alias
- `KEY_PASSWORD` → كلمة مرور المفتاح
- `STORE_PASSWORD` → كلمة مرور المتجر

```bash
# لإنشاء keystore جديد:
keytool -genkey -v -keystore my-release-key.keystore \
  -alias currency-pro -keyalg RSA -keysize 2048 -validity 10000

# تحويل الملف إلى base64:
base64 -i my-release-key.keystore | pbcopy
```

---

## 📱 تثبيت APK على الهاتف

1. فعّل **مصادر غير معروفة** في إعدادات الهاتف
2. انقل ملف APK إلى هاتفك
3. اضغط عليه وثبّته

---

## 🛠️ التطوير المحلي

```bash
# تثبيت خادم محلي بسيط
npx serve .

# أو استخدم Python
python -m http.server 8080
```

---

## 📄 الرخصة

MIT License © 2024 Currency Converter Pro
