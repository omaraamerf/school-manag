# تقسيم المشروع (Issues + Milestones)

هذا الملف جاهز لنسخه إلى GitHub Issues/Milestones/Project Board.

## الأدوار
- Omar Amer (PM/Lead): إدارة GitHub + الدمج + المتابعة
- Hazem (UI/Template): تخطيط الواجهة + RTL + Navigation
- Ali Husen (Students): الطلاب + ملف الطالب
- Mustafa baaj (Teachers/Classes): المعلمين + الفصول/المواد
- Ebrahim hamo (Attendance/Grades/Fees + QA): الحضور + الدرجات + الرسوم + اختبار

## Labels المقترحة
- النوع: `type:feature`, `type:bug`, `type:task`, `type:docs`
- المجال: `area:ui`, `area:students`, `area:teachers`, `area:classes`, `area:attendance`, `area:grades`, `area:fees`, `area:auth`
- الأولوية: `priority:high`, `priority:medium`, `priority:low`

## Milestones (مراحل للمقرر)
- M1: أساس المشروع (Repo/Workflow/UI Skeleton)
- M2: إدارة الأكاديمية (طلاب/معلمين/فصول)
- M3: العمليات (حضور/درجات/رسوم)
- M4: التجهيز للعرض (توثيق/QA/عرض نهائي)

---

## M1 — أساس المشروع (Repo/Workflow/UI Skeleton)

### 1) [Task] إعداد المستودع وسياسة الفروع
- **Assignee:** Omar Amer
- **Labels:** `type:task`, `priority:high`
- **Acceptance:**
  - Branch protection على `main`
  - إنشاء `develop`
  - تفعيل PR review (1 على الأقل)

### 2) [Task] إنشاء GitHub Project Board + Labels + Milestones
- **Assignee:** Omar Amer
- **Labels:** `type:task`, `priority:high`
- **Acceptance:**
  - Board بالأعمدة (Backlog/Ready/In Progress/In Review/Done)
  - Labels مضافة
  - Milestones مضافة (M1..M4)

### 3) [Docs] إعداد README (وصف المشروع + طريقة التشغيل)
- **Assignee:** Omar Amer
- **Labels:** `type:docs`, `priority:medium`
- **Acceptance:**
  - README يحتوي: فكرة المشروع، الصفحات، طريقة فتح `dist/index.html`

### 4) [Feature] توحيد التنقل (Sidebar/Topbar) في كل الصفحات
- **Assignee:** Hazem
- **Labels:** `type:feature`, `area:ui`, `priority:high`
- **Acceptance:**
  - كل صفحة فيها نفس Sidebar/Topbar
  - الروابط تعمل وتفتح صفحات النظام فقط

### 5) [Feature] RTL + تحسين الخطوط والنصوص العربية
- **Assignee:** Hazem
- **Labels:** `type:feature`, `area:ui`, `priority:medium`
- **Acceptance:**
  - اتجاه RTL ثابت
  - عناوين عربية متسقة

### 6) [Bug] مراجعة أخطاء Console في كل الصفحات
- **Assignee:** Ebrahim hamo
- **Labels:** `type:bug`, `priority:high`
- **Acceptance:**
  - لا توجد أخطاء Console عند فتح الصفحات الرئيسية

---

## M2 — إدارة الأكاديمية (طلاب/معلمين/فصول)

### 7) [Feature] صفحة الطلاب: جدول + بحث/فلترة (واجهة)
- **Assignee:** Ali Husen
- **Labels:** `type:feature`, `area:students`, `priority:high`
- **Acceptance:**
  - حقول بحث/فلترة واضحة
  - جدول منسق + بيانات تجريبية

### 8) [Feature] صفحة الطلاب: Modal إضافة/تعديل (واجهة)
- **Assignee:** Ali Husen
- **Labels:** `type:feature`, `area:students`, `priority:high`
- **Acceptance:**
  - Modal إضافة موجود
  - زر “تعديل” يفتح Modal (حتى لو بدون حفظ فعلي)

### 9) [Feature] صفحة ملف الطالب: تبويب/أقسام (معلومات + درجات + فواتير)
- **Assignee:** Ali Husen
- **Labels:** `type:feature`, `area:students`, `priority:medium`
- **Acceptance:**
  - عرض معلومات الطالب بشكل بطاقة/أقسام
  - روابط إلى الدرجات/الرسوم تعمل

### 10) [Feature] صفحة المعلمين: جدول + بحث/فلترة (واجهة)
- **Assignee:** Mustafa baaj
- **Labels:** `type:feature`, `area:teachers`, `priority:high`
- **Acceptance:**
  - جدول بيانات تجريبية
  - فلترة/بحث واجهة

### 11) [Feature] صفحة المعلمين: Modal إضافة/تعديل (واجهة)
- **Assignee:** Mustafa baaj
- **Labels:** `type:feature`, `area:teachers`, `priority:medium`
- **Acceptance:**
  - Modal إضافة موجود
  - أزرار تعديل/حذف شكلية

### 12) [Feature] صفحة الفصول: إدارة الفصول (واجهة)
- **Assignee:** Mustafa baaj
- **Labels:** `type:feature`, `area:classes`, `priority:high`
- **Acceptance:**
  - جدول فصول + أزرار تعديل
  - Modal إضافة فصل

### 13) [Feature] صفحة المواد: إدارة المواد وربطها بفصل/معلم (واجهة)
- **Assignee:** Mustafa baaj
- **Labels:** `type:feature`, `area:classes`, `priority:high`
- **Acceptance:**
  - جدول مواد + اختيار فصل + بحث
  - Modal إضافة مادة

---

## M3 — العمليات (حضور/درجات/رسوم)

### 14) [Feature] صفحة الحضور: تحميل قائمة + حفظ (واجهة)
- **Assignee:** Ebrahim hamo
- **Labels:** `type:feature`, `area:attendance`, `priority:high`
- **Acceptance:**
  - اختيار تاريخ/فصل
  - جدول حضور (حاضر/غائب) + حقل ملاحظة

### 15) [Feature] صفحة الدرجات: اختيار فصل/مادة + إدخال درجات (واجهة)
- **Assignee:** Ebrahim hamo
- **Labels:** `type:feature`, `area:grades`, `priority:high`
- **Acceptance:**
  - جدول درجات بمدخلات رقمية
  - مجموع/تقدير (حتى لو ثابت/عرضي)

### 16) [Feature] صفحة الرسوم: قائمة فواتير + إنشاء فاتورة (واجهة)
- **Assignee:** Ebrahim hamo
- **Labels:** `type:feature`, `area:fees`, `priority:high`
- **Acceptance:**
  - فلترة حسب الحالة + بحث
  - Modal إنشاء فاتورة

### 17) [Feature] صفحة الإعدادات: نموذج بيانات المدرسة (واجهة)
- **Assignee:** Hazem
- **Labels:** `type:feature`, `area:ui`, `priority:medium`
- **Acceptance:**
  - نموذج منسق + أزرار حفظ/إلغاء شكلية

### 18) [Feature] صفحة تسجيل الدخول (واجهة) وربطها من القائمة
- **Assignee:** Hazem
- **Labels:** `type:feature`, `area:auth`, `priority:medium`
- **Acceptance:**
  - صفحة دخول واجهة فقط
  - الروابط من جميع الصفحات تشير لها

---

## M4 — التجهيز للعرض (توثيق/QA/عرض نهائي)

### 19) [QA] تدقيق الروابط: لا روابط لصفحات محذوفة
- **Assignee:** Ebrahim hamo
- **Labels:** `type:task`, `priority:high`
- **Acceptance:**
  - فحص شامل للتنقل في كل الصفحات

### 20) [QA] تدقيق اللغة العربية وتوحيد المصطلحات
- **Assignee:** Hazem
- **Labels:** `type:task`, `priority:medium`
- **Acceptance:**
  - توحيد المصطلحات (طلاب/معلمين/فصول/مواد/رسوم/حضور/درجات)

### 21) [Docs] توثيق بنمط SRS مختصر (هدف/نطاق/أدوار/صفحات)
- **Assignee:** Omar Amer
- **Labels:** `type:docs`, `priority:high`
- **Acceptance:**
  - ملف واحد أو قسم في README يشرح المتطلبات والصفحات

### 22) [Docs] دليل العرض النهائي (Demo Script)
- **Assignee:** Omar Amer
- **Labels:** `type:docs`, `priority:medium`
- **Acceptance:**
  - خطوات عرض (دخول → لوحة → طلاب → ملف → حضور → درجات → رسوم)

### 23) [Release] إصدار نهائي v1.0
- **Assignee:** Omar Amer
- **Labels:** `type:task`, `priority:high`
- **Acceptance:**
  - دمج `develop` إلى `main`
  - Tag/Release: `v1.0`

