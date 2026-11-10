# Dazai Player

مشغل موسيقى خفيف بواجهة عربية، يمسح الملفات الصوتية ويعرض المكتبة والإحصاءات والإعدادات. يحفظ فهرس المكتبة محليًا، ويمكن تغليفه كتطبيق Android عبر Capacitor.

هذا المستودع مبني على مشروع `vfhghhfy/Dazai-Player`.

## المتطلبات

- Node.js 20 أو أحدث وnpm.
- لبناء Android: Android Studio وAndroid SDK وJDK 17 أو أحدث.

## التثبيت والتشغيل على الويب

```bash
git clone https://github.com/haiderbyte/Dazai-Player.git
cd Dazai-Player
npm install
npm run dev
```

افتح عنوان Vite المحلي الذي يظهر في الطرفية.

## التحقق والبناء

```bash
npm run lint       # فحص TypeScript
npm run build      # بناء نسخة الويب داخل dist/
npm run preview    # معاينة نسخة الإنتاج
```

## إعداد Android

إذا لم يكن مجلد `android/` موجودًا، أضف مشروع Android مرة واحدة:

```bash
npm run cap:add
```

بعد ذلك ابنِ ملفات الويب وزامنها مع Android:

```bash
npm run build:android
npx cap open android
```

أكمل بناء APK أو تشغيل التطبيق من Android Studio. لا يلزم مفتاح Gemini؛ تعليمات AI Studio القديمة لم تعد تخص هذا المشروع.
