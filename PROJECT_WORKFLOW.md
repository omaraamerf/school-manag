# خطة العمل على GitHub (فريق 5 أشخاص)

## ملف التقسيم الجاهز
تم تجهيز تقسيم كامل (Milestones + Issues + توزيع على 5 أشخاص) داخل الملف:
- [GITHUB_BACKLOG.md](file:///c:/Users/sthla/OneDrive/Desktop/HTML/GITHUB_BACKLOG.md)

## 1) إعداد المستودع (مرة واحدة)
1. إنشاء Repository باسم مناسب مثل: `school-system-frontend`.
2. إضافة أعضاء الفريق كـ Collaborators (صلاحية Write).
3. تفعيل Branch Protection على فرع `main`:
   - منع الـ direct push إلى `main`.
   - إلزام Pull Request قبل الدمج.
   - إلزام Review واحد على الأقل قبل الدمج.
4. إنشاء فرع `develop`
   - `main`: نسخة مستقرة/عرض نهائي.
   - `develop`: تجميع ميزات الفريق قبل إصدار نسخة للعرض.

## 2) سياسة الفروع (Branches)
- `main`: لا يُدمج فيه إلا عبر PR من `develop`.
- `develop`: يُدمج فيه عبر PR من فروع الميزات.
- `feature/<module>-<short>`: ميزات جديدة (مثال: `feature/students-table`).
- `fix/<short>`: إصلاحات (مثال: `fix/sidebar-active-link`).
- `docs/<short>`: توثيق فقط.

## 3) طريقة العمل القياسية (Issue → Branch → PR)
1. إنشاء Issue لكل مهمة (Feature/Bug/Task) بعنوان واضح.
2. تحويل الـ Issue إلى مهمة داخل GitHub Project (Board) jira.
3. إنشاء فرع من `develop` مرتبط بالمهمة:
   - اسم الفرع يحتوي رقم الـ Issue: `feature/12-students-filter`.
4. تنفيذ التغيير + Commitات صغيرة (1 فكرة = 1 Commit).
5. فتح Pull Request إلى `develop` وربطه بالـ Issue:
   - في وصف الـ PR اكتب: `Closes #12` لإغلاق الـ Issue تلقائيًا بعد الدمج.
6. Review من زميل واحد على الأقل ثم Merge.
7. عند نهاية Sprint/مرحلة: عمل PR من `develop` إلى `main` باسم `Release v0.1`.

## 4) مشروع GitHub (Project Board)
- Ready
- In Progress
- In Review
- Done

## 5) Milestones (مراحل/سبرنت)
- Milestone 1: UI Skeleton + Navigation
- Milestone 2: Students + Teachers + Classes
- Milestone 3: Attendance + Grades + Fees
- Milestone 4: Polish + Demo + Documentation

## 6) معايير قبول المهمة (Definition of Done)
أي Issue تعتبر “Done” إذا:
- تم ربطها بـ PR وتمت مراجعة الـ PR.
- لا توجد أخطاء Console في الصفحات المرتبطة بالمهمة.
- الروابط والتنقل يعمل.
- تحديث README/توثيق بسيط إذا لزم.

## 7) توزيع الأدوار (5 أشخاص) —  
### (أ) قائد/PM + إعداد GitHub
- إعداد المستودع والفروع والـ Project Board والـ Labels.
- تقسيم المتطلبات إلى Issues.
- التأكد من الالتزام بالـ PR/Review.

### (ب) مسؤول الواجهة العامة/التخطيط
- تحسين القائمة الجانبية، الـ Topbar، التوافق RTL، وتجربة المستخدم.
- توحيد شكل الجداول/النماذج (Cards, Tables, Modals).

### (ج) مسؤول الطلاب
- صفحات الطلاب + ملف الطالب + نماذج (Add/Edit).
- عينات بيانات (Mock) وتحسين العرض.

### (د) مسؤول المعلمين + الفصول/المواد
- صفحات المعلمين.
- صفحات الفصول/المواد وربطها بالواجهة.

### (هـ) مسؤول الحضور + الدرجات + الرسوم + QA
- صفحات الحضور/الدرجات/الرسوم.
- QA: اختبار التنقل، فحص الأخطاء، توحيد نصوص اللغة.
- تجهيز عرض المشروع (Demo checklist).

## 8) Labels مقترحة (للتقييم والوضوح)
- `type:feature`, `type:bug`, `type:task`, `type:docs`
- `area:students`, `area:teachers`, `area:classes`, `area:attendance`, `area:grades`, `area:fees`, `area:ui`
- `priority:high`, `priority:medium`, `priority:low`
- `status:blocked`

## 9) قالب أسماء الـ Commits (مبسّط)
- `feat: ...` ميزة
- `fix: ...` إصلاح
- `docs: ...` توثيق
- `chore: ...` تنظيف/ترتيب

## 10) محاكاة “إدارة مشروع” داخل GitHub (كيف تُظهرونها للمقرر)
1. أنشئ Issues لكل ميزة (مع Acceptance Criteria).
2. ضع Issues داخل Milestones.
3. حرّكها في Project Board حسب تقدم الفريق.
4. اربط كل PR بـ Issue وأظهر الـ Review والتعليقات.
5. اعمل Release Tags بسيطة: `v0.1`, `v0.2` (حتى لو Front فقط).
