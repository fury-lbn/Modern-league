# دوري مدرسة النظم الحديثة الكروي — Modern Systems School

## محتويات المشروع
- `index.html`: الموقع الكامل (الواجهة الأمامية + لوحة الإدارة + اللغتان AR/EN + المجسم ثلاثي الأبعاد).
- `config.js`: ملف الإعدادات الوحيد الذي تضع فيه مفاتيح Supabase ورابط الديسكورد.
- `assets/pulse_football_v1.glb`: المجسم ثلاثي الأبعاد المتحرك للواجهة الرئيسية.
- `sql/supabase_schema.sql`: كود إنشاء جداول قاعدة البيانات والصلاحيات (RLS) والبث اللحظي (Realtime).
- `.nojekyll`: لضمان تشغيل الملفات فورًا على GitHub Pages.

## خطوات التشغيل السريعة
1. أنشئ مشروعًا جديدًا على [Supabase](https://supabase.com)، افتح **SQL Editor**، الصق محتوى `sql/supabase_schema.sql` واضغط **Run**.
2. من **Authentication → Users** اضغط **Add User** وأنشئ حساب المشرف الأول (بريد إلكتروني + كلمة مرور).
3. من **Project Settings → API** انسخ `Project URL` و`anon public` key والصقهما داخل ملف `config.js`.
4. أنشئ مستودعًا (Repository) جديدًا على [GitHub](https://github.com) وارفع جميع ملفات المجلد كما هي.
5. من **Settings → Pages** اختر الفرع `main` والمجلد `/ (root)` ثم اضغط **Save** ليصبح موقعك مباشرًا خلال دقيقة.
