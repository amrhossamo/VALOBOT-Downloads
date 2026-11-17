# VALOBOT — Windows downloads

VALOBOT is a desktop workspace for managing your Eldorado Valorant boosting offers.

## Download

[Download the latest VALOBOT for Windows x64](https://github.com/amrhossamo/VALOBOT-Downloads/releases/latest):

- **Setup**: installs VALOBOT and creates shortcuts.
- **Portable**: runs without a separate Node.js installation.
SHA256SUMS.txt contains the checksums for both downloads.

An account activated by your administrator is required. There is no public signup or payment checkout. Subscription payments and renewal are handled directly with the administrator.

## Updates and settings

If you have 1.0.0, download and install the new **Setup once**. Starting with 1.1.0, the installed app checks GitHub Releases after launch and downloads newer versions in the background. Choose **Restart and update** after stopping the bot. Installation is blocked while the bot is running or busy, or if saving settings fails. Portable updates remain manual.

Prices, filters, server rank limits and Solo/Duo messages persist on the Windows device per VALOBOT account across updates. **General Settings → Settings backup** exports/imports a JSON backup. Backups do not include passwords, Eldorado credentials or login tokens. Keep a backup before moving to a different device.

The updater follows the public GitHub release manifest and verifies installer checksums. Initial builds remain unsigned; a manual update round-trip on a separate clean customer PC has not yet been completed.

## Account protection

Each customer account is locked to the first Eldorado Seller API account connected through VALOBOT. Disconnecting or reinstalling does not reset that server-side link. A change requires explicit administrator approval. Another customer login ends the earlier session at its next verification. No device-specific lock is used.

## Features

- Arabic and English interface.
- Readiness checks before starting live offers.
- Rank Boost, Net Wins and Placements pricing from your settings.
- Base prices, server surcharges and a Duo surcharge percentage.
- Separate Solo and Duo messages.
- Request previews that never submit an offer.
- Clear skip reasons with shortcuts to the relevant settings.
- Automatic settings saves, optional notifications and subscription reminders.
- Optional Eldorado inbox for manual replies.

Eldorado credentials and pricing are stored on your device. Saved Eldorado login uses Windows DPAPI. The subscription service stores VALOBOT account and license information plus a one-way seller-binding fingerprint and short reference. Your Eldorado Client Secret stays on your device.

The bot requires an active subscription, valid Eldorado Seller API access, an internet connection and a running device. New request checks run every five seconds; Eldorado response time also affects delivery of an offer. Closing the app stops the bot unless you choose to minimize it to the tray.

Early builds are unsigned. SHA-256 checksums accompany published downloads. This repository distributes downloads and documentation; the application and subscription-service source are not published here.

---

## بالعربي

حمّل النسخة المناسبة من **Releases**. نسخة Setup للتثبيت، وPortable للتشغيل المحمول. مش محتاج تثبّت Node.js.

سجّل دخولك بالحساب الذي استلمته من الأدمن، ثم اربط حساب Eldorado، وحدد أسعارك ومددك ورسائلك. اعمل فحص الجاهزية قبل تشغيل العروض الحقيقية. الدفع والتجديد خارج البرنامج عن طريق الأدمن.

المعاينة لا ترسل عروضًا. الخانات غير المسعّرة والطلبات خارج فلاترك يتم تخطيها بسبب ظاهر في سجل النشاط. تغيير الأسعار أثناء عمل البوت يُحفظ، لكنه يحتاج إيقاف البوت وتشغيله ليُطبَّق على الإرسال.

الإصدارات الأولى غير موقّعة رقميًا. حسابات العملاء وبيانات Eldorado ومفاتيح إدارة الخدمة لا تُنشر في هذا المستودع.

حساب العميل مرتبط بحساب Eldorado واحد ثابت. فصل الحساب أو إعادة تثبيت البرنامج لا يلغي الربط؛ التغيير من صلاحية الأدمن فقط. تسجيل الدخول من نسخة أخرى ينهي الجلسة السابقة عند التحقق التالي.


للتحديث من 1.0.0: حمّل نسخة Setup الجديدة وثبّتها مرة واحدة. بعدها التحديثات القادمة تُنزّل من داخل البرنامج، والتثبيت بعد إيقاف البوت وحفظ الإعدادات. من الإعدادات العامة تقدر تعمل استيراد وتصدير لأسعارك وفلاترك ورسائلك؛ النسخة الاحتياطية لا تحتوي على الباسوردات أو مفاتيح Eldorado.
