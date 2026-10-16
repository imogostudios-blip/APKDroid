# APKDroid Store

هذه النسخة تعتمد على `src/app.js` بوصفه ملف التطبيق الوحيد وقت التشغيل، ولا تحتاج إلى `app.jsx` أو Babel أو خطوة بناء داخل المتصفح.

## ملفات التشغيل الأساسية
- `index.html`: يحمّل React وReactDOM المحليين ثم `src/app.js`.
- `src/app.js`: كود التطبيق الفعلي الذي يعمل في المتصفح.
- `src/styles/app.css` و`src/styles/tailwind.css`: تنسيقات الواجهة.
- `sw.js`: يخزّن غلاف التطبيق للعمل دون اتصال بعد أول زيارة ناجحة.

## التشغيل
شغّل خادمًا محليًا من مجلد المشروع، مثلًا:

```bash
python3 -m http.server 8080
```

ثم افتح `http://localhost:8080`. لا تفتح `index.html` مباشرةً عبر `file://` لأن Service Worker وبعض ميزات المتصفح تحتاج إلى HTTP أو HTTPS.

البحث والتنزيل من الخدمات الخارجية يتطلبان اتصالًا بالإنترنت.


## Latest UI updates
- Settings opens directly without the previous onboarding or settings loading screen.
- App detail metadata is presented as a strip above the install action.
- Sharing uses the browser/operating-system native share interface when supported, sharing a Google Play search URL for the app name.
- The style toggle uses the accessible teal switch design.
- Service-worker cache version: apkdroid-v18.
