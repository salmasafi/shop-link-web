# تحميل خطوط Cairo

## الخطوات المطلوبة:

يجب تحميل ملفات الخطوط التالية ووضعها في مجلد `assets/fonts/`:

### الطريقة 1: التحميل من Google Fonts GitHub (موصى بها)

قم بتحميل الملفات التالية من المستودع الرسمي:

```
https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-Regular.ttf
https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-Medium.ttf
https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-SemiBold.ttf
https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-Bold.ttf
https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-ExtraBold.ttf
https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-Black.ttf
```

### الطريقة 2: استخدام الأوامر (Windows PowerShell)

افتح PowerShell في مجلد المشروع وقم بتشغيل:

```powershell
cd assets\fonts

# تحميل الخطوط
Invoke-WebRequest -Uri "https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-Regular.ttf" -OutFile "Cairo-Regular.ttf"
Invoke-WebRequest -Uri "https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-Medium.ttf" -OutFile "Cairo-Medium.ttf"
Invoke-WebRequest -Uri "https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-SemiBold.ttf" -OutFile "Cairo-SemiBold.ttf"
Invoke-WebRequest -Uri "https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-Bold.ttf" -OutFile "Cairo-Bold.ttf"
Invoke-WebRequest -Uri "https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-ExtraBold.ttf" -OutFile "Cairo-ExtraBold.ttf"
Invoke-WebRequest -Uri "https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-Black.ttf" -OutFile "Cairo-Black.ttf"

cd ..\..
```

### الطريقة 3: استخدام curl (إذا كان متوفراً)

```bash
cd assets/fonts
curl -L -o Cairo-Regular.ttf "https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-Regular.ttf"
curl -L -o Cairo-Medium.ttf "https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-Medium.ttf"
curl -L -o Cairo-SemiBold.ttf "https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-SemiBold.ttf"
curl -L -o Cairo-Bold.ttf "https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-Bold.ttf"
curl -L -o Cairo-ExtraBold.ttf "https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-ExtraBold.ttf"
curl -L -o Cairo-Black.ttf "https://github.com/google/fonts/raw/main/ofl/cairo/Cairo-Black.ttf"
cd ../..
```

## بعد التحميل:

1. تأكد من وجود جميع الملفات الستة في مجلد `assets/fonts/`
2. قم بتشغيل: `flutter clean`
3. قم بتشغيل: `flutter pub get`
4. جرب تشغيل التطبيق مرة أخرى

## الملفات المطلوبة:
- ✅ Cairo-Regular.ttf (400)
- ✅ Cairo-Medium.ttf (500)
- ✅ Cairo-SemiBold.ttf (600)
- ✅ Cairo-Bold.ttf (700)
- ✅ Cairo-ExtraBold.ttf (800)
- ✅ Cairo-Black.ttf (900)
