# ملفات Celyah Robot الكاملة – آخر نسخة مجمّعة

## تطبيق Flutter
- `lib/main.dart`: واجهة التطبيق والتحكم بالضغط المستمر (V2).
- `lib/robot_link.dart`: الاتصال عبر BLE.
- `lib/gemini_client.dart`: الاتصال بـ Gemini.
- `lib/face_frame_stream.dart`: عرض صورة وجه الروبوت.
- `pubspec.yaml`: الاعتمادات.
- `assets/branding/`: صور الهوية.
- `tools/`: أدوات إعداد Android والهوية.
- `.github/workflows/build_apk.yml`: بناء APK وإرفاقه في Artifacts، مع ضبط مكتبة BLE وSDK 36.

## كود الروبوت
- `ESP32/Celyah_Robot_Hybrid/Celyah_Robot_Hybrid.ino`
- `ESP32/Celyah_Robot_Hybrid/CelYah_Types.h`

## طريقة الرفع
1. ارفع ملفات تطبيق Flutter إلى جذر مستودع GitHub، مع الاحتفاظ ببنية المجلدات.
2. ارفع ملفات مجلد ESP32 معًا من Arduino IDE.
3. شغّل GitHub Actions وتأكد من ظهور خطوتي Build release APK وUpload APK.

## تنبيه مهم
هذه حزمة تجميع لأحدث الملفات الموجودة من العمل السابق، وليست نسخة تم التأكد من تجميعها أو اختبارها على الأجهزة. قد تتطلب بعض الإعدادات أو إصلاحات التوافق. لا تضع مفتاح Gemini السري في GitHub. افحص حركة العجل بأمان بعيدًا عن الحواف.
