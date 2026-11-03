تطبيق مكة للمجوهرات - مشروع Android

مهم:
هذه ملفات مشروع Android Studio وليست APK جاهزاً للتثبيت. بيئة إنشاء الملفات الحالية لا تحتوي على Android SDK أو Gradle، لذلك لم أتمكن من بناء APK واختباره هنا.

طريقة إنشاء APK:
1) ثبّت Android Studio على كمبيوتر.
2) فك ضغط MakkaJewelryAndroid.zip.
3) من Android Studio اختر Open وافتح مجلد MakkaJewelryAndroid.
4) انتظر Gradle Sync وثبّت Android SDK Platform 35 إذا طلبه البرنامج.
5) من القائمة اختر Build > Build Bundle(s) / APK(s) > Build APK(s).
6) بعد انتهاء البناء اضغط Locate للوصول إلى ملف APK.

التطبيق يفتح ملف HTML المرفق داخلياً داخل WebView، مع تفعيل JavaScript والتخزين المحلي واختيار الملفات لاسترجاع النسخ الاحتياطية.
بيانات localStorage تبقى على نفس تثبيت التطبيق؛ لا تحذف التطبيق أو بياناته دون وجود نسخة احتياطية.
تصدير Excel في الملف الحالي يعتمد على مكتبة SheetJS من CDN، ولذلك يحتاج اتصال إنترنت عند التصدير لأول مرة/عند عدم توفر المكتبة مخزنة.
