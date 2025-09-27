# بقشتي - تطبيق إدارة الحسابات المالية

<div dir="rtl">

## 📱 نظرة عامة

**بقشتي** هو تطبيق متكامل لإدارة الحسابات المالية الشخصية والمؤسسية بنظام هرمي متقدم. يساعدك على تنظيم أموالك ومتابعة معاملاتك المالية بسهولة وأمان.

---

## ✨ المميزات

### 💼 إدارة الحسابات الهرمية

* إنشاء حسابات رئيسية وفرعية
* هيكلة مالية متعددة المستويات
* تصنيف الحسابات (أصول، خصوم، إيرادات، مصروفات)

### 💳 نظام المعاملات المتكامل

* تسجيل عمليات الإيداع والسحب
* تتبع الحركات المالية بشكل زمني
* إرفاق وصف ومرجع لكل معاملة

### 📊 تقارير وإحصائيات

* لوحة تحكم شاملة بالإحصائيات
* تقارير مالية متنوعة
* رسوم بيانية توضيحية
* تقارير حسب الفترات الزمنية

### 🔐 الأمان والخصوصية

* نظام تسجيل دخول آمن
* تشفير كلمات المرور
* عزل بيانات المستخدمين
* واجهة عربية بالكامل

---

## 🛠 التقنيات المستخدمة

* **Flutter 3.35.4+** – إطار العمل الرئيسي
* **Dart 3.9.2+** – لغة البرمجة
* **SQLite** – قاعدة البيانات المحلية
* **Provider** – إدارة الحالة
* **Shared Preferences** – التخزين المحلي

---

## 📥 التثبيت والتشغيل

### المتطلبات الأساسية

* Flutter SDK 3.35.4 أو أعلى
* Dart SDK 3.9.2 أو أعلى
* Android Studio / VS Code

### خطوات التشغيل

```bash
# 1. Clone المشروع
git clone https://github.com/26ajd/biqishati.git

# 2. انتقل للمجلد
cd parent_account_guide

# 3. ثبّت dependencies
flutter pub get

# 4. شغّل التطبيق
flutter run
```

### بناء التطبيق للإصدار

```bash
# بناء APK للأندرويد
flutter build apk --release

# بناء App Bundle
flutter build appbundle --release

# بناء iOS (يتطلب macOS)
flutter build ios --release
```

---

## 🏗 هيكل المشروع

```
lib/
├── models/          # 📊 نماذج البيانات
│   ├── account.dart
│   ├── transaction.dart
│   └── user.dart
├── services/        # ⚙️ الخدمات والمنطق
│   ├── database_service.dart
│   ├── account_service.dart
│   ├── transaction_service.dart
│   └── auth_service.dart
├── repositories/    # 🗃 طبقة الوصول للبيانات
│   ├── account_repository.dart
│   ├── transaction_repository.dart
│   └── user_repository.dart
├── providers/       # 🎛 إدارة الحالة
│   ├── auth_provider.dart
│   ├── account_provider.dart
│   └── transaction_provider.dart
├── screens/         # 🖥 شاشات التطبيق
│   ├── auth/        # شاشات التسجيل
│   ├── home/        # الشاشة الرئيسية
│   ├── accounts/    # إدارة الحسابات
│   └── reports/     # التقارير والإحصائيات
├── widgets/         # ⚡️ مكونات واجهة مستخدم
│   ├── dashboard_card.dart
│   ├── recent_transactions_widget.dart
│   └── report_chart.dart
└── utils/           # 🛠 أدوات مساعدة
    ├── app_theme.dart
    ├── date_utils.dart
    └── currency_utils.dart
```

---

## 📦 dependencies المستخدمة

```yaml
dependencies:
  flutter:
    sdk: flutter
  cupertino_icons: ^1.0.6
  sqflite: ^2.3.0        # قاعدة بيانات SQLite
  path: ^1.8.3           # التعامل مع المسارات
  intl: ^0.19.0          # التنسيق الدولي
  crypto: ^3.0.3         # التشفير
  shared_preferences: ^2.2.2 # التخزين المحلي
  provider: ^6.1.1       # إدارة الحالة

dev_dependencies:
  flutter_test:
    sdk: flutter
  flutter_lints: ^3.0.0
```

---

## 🎨 الهوية البصرية

* **الألوان الأساسية:** أزرق (#1976D2) + أسود (#212121)
* **النمط:** Material Design 3
* **اللغة:** العربية (دعم كامل RTL)

---

## 🔄 حالات الاستخدام

### للمستخدم الفردي

* تتبع المصروفات الشخصية
* إدارة المدخرات والاستثمارات
* مراقبة التدفقات النقدية

### للشركات الصغيرة

* إدارة حسابات المؤسسة
* متابعة الإيرادات والمصروفات
* تقارير مالية مبسطة

### للمحاسبين

* هيكلة الحسابات بشكل هرمي
* تسجيل القيود اليومية
* إصدار تقارير مالية

</div>
