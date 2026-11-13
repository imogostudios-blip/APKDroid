ضع الصور هنا بأسمائها فقط:  apps1.png , apps2.jpg , games1.webp ...
  appsN  -> تحت سطر التطبيقات رقم N في الصفحة الرئيسية
  gamesN -> تحت سطر الألعاب رقم N في صفحة الألعاب

الرابط والاسم (اختياريان) يُكتبان في photos.xml بهذا الشكل:
</photos>
</apps1>
<url=https://example.com>
<name=هون الاسم>
</end>
</apps2>
<url=https://example.com>
</end>
</games1>
<name=الاسم هون>
</end>

ملاحظة: اكتب كل صورة في photos.xml (حتى لو بدون رابط/اسم: </apps3> ثم </end>) لتضمن ظهورها على أي استضافة.
