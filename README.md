# بوابة تصاريح الأعمال – تعليمات نشر سريعة

> تم الإنشاء: 2025-10-28 16:39

يحتوي هذا المجلّد على:
- `index.html` (الملف الرئيسي)
- `404.html` (نسخة مطابقة كاحتياط)
- ملفات خارجية عبر CDN (Tailwind + qrcodejs) – لا حاجة لبناء.

## 1) GitHub Pages (مجاني، موثوق)
1. أنشئ حسابًا على GitHub (إن لم يكن لديك).
2. أنشئ مستودعًا جديدًا باسم مثل: `ptw-portal` (عام Public).
3. ارفع `index.html` و`404.html` في **الجذر**.
4. من `Settings → Pages`:  
   - **Source** = `Deploy from a branch`  
   - **Branch** = `main` و **Folder** = `/root` ثم **Save**.
5. انتظر دقيقة ثم افتح الرابط:  
   `https://USERNAME.github.io/ptw-portal/`

> إن ظهرت 404: تأكد أن `index.html` في الجذر وأن الإعدادات محفوظة.

## 2) Cloudflare Pages (CDN سريع جدًا – مجاني)
1. أنشئ حسابًا على Cloudflare.
2. من **Pages** اختر **Create a project** ثم **Connect to Git** واختر نفس Repo.
3. إعدادات البناء:  
   - Framework: `None`  
   - Build command: *(فارغ)*  
   - Output directory: `/`  
4. Deploy وستحصل على نطاق `*.pages.dev`.

## 3) Vercel (سهل مع GitHub)
1. سجل دخولًا على Vercel.
2. **New Project → Import** مستودع GitHub.
3. Framework: `Other`، بدون Build command، Output = `/`.
4. Deploy واحصل على نطاق `*.vercel.app`.

> ملاحظة: صور الخلفية/الشعار من Google Drive، تأكد أن مشاركة الملف `Anyone with the link` لظهورهما للجميع.
