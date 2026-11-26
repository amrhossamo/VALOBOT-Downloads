# AutoOffer — Windows downloads

AutoOffer is a Windows desktop workspace for managing your Eldorado League of Legends boosting offers. The current edition supports League only.

Previously named VALOBOT. Existing installations receive AutoOffer through the same update feed; saved settings and account data keep their existing profile location.

## Download

[Download the latest AutoOffer for Windows x64](https://github.com/amrhossamo/VALOBOT-Downloads/releases/latest):

- **Setup**: installs AutoOffer and creates shortcuts.
New releases provide **Setup only**, with automatic-update support. SHA256SUMS.txt contains installer and updater-file checksums.

An account activated by your administrator is required. There is no public signup or payment checkout. Subscription payments and renewal are handled directly with the administrator.

## Updates and settings

If you have 1.0.0, download and install the new **Setup once**. Starting with 1.1.0, the installed app checks GitHub Releases after launch and downloads newer versions in the background. Choose **Restart and update** after stopping the bot. Installation is blocked while the bot is running or busy, or if saving settings fails. Portable updates remain manual.

Prices, filters, server rank limits and Solo/Duo messages persist on the Windows device per AutoOffer account across updates. **General Settings → Settings backup** exports/imports a JSON backup. Backups do not include passwords, Eldorado credentials or login tokens. Keep a backup before moving to a different device.

The updater follows the public GitHub release manifest and verifies installer checksums. Initial builds remain unsigned; a manual update round-trip on a separate clean customer PC has not yet been completed.

## Account protection

Each customer account is locked to a verified Eldorado seller account ID. AutoOffer verifies Eldorado’s signed short-lived access token against its official public keys; a new API key for the same seller is accepted, while a different seller requires administrator approval. The license service stores an account hash, not the identity token or Client Secret. Legacy client-key locks migrate after proof from the old key; if that key is unavailable, the administrator must approve the migration. Administrator approval for a seller change preserves the customer login, but an explicit Connect is required to verify the replacement seller. Connect always checks again, even for the same API key. A genuinely revoked login returns to the sign-in screen without erasing saved seller credentials. Another customer login ends the earlier session at its next verification. No device-specific lock is used. Remembered AutoOffer login lasts up to 30 days; expiry, revocation and suspension still apply.

## League workspace

The app runs one League engine. Existing League prices, messages and saved Seller API credentials stay in their previous profile location. Old game settings are not deleted. Your administrator manages League access; connecting your seller still requires a valid signed identity.

## Features

- Arabic and English interface.
- Readiness checks before starting live offers.
- Rank Boost, Net Wins and Placements pricing from your settings, with hours-only durations for every rank (per match for Net Wins/Placements).
- Base prices, server surcharges and a Duo surcharge percentage.
- Separate Solo and Duo offer comments. Follow-up chat sends each nonempty line as its own message, followed by selected images.
- Per-server Duo permissions; Solo continues to use the main server selection.
- Optional one-time no-reply reminder with your text and delay. Any customer reply after the first chat messages cancels it permanently. Closing/restarting/stopping or losing reply verification suppresses the reminder.
- Inbox request details, verified order status, your submitted offer price and configured/rounded delivery, separate from the paid order total. Unknown payment states remain unknown.
- Simple English Live Activity with start/stop, successful offers and clear failure reasons.
- Distinct missing-price and missing-duration errors, plus a warning when saved settings differ from active bot rules.
- Separate Net Wins and Placements tables.
- Configurable League Rank Boost discount above 30 LP; 0% disables it.
- League regions: EUW, EUNE, NA, ME, LAN, LAS and TR.
- Fixed inbox layout with message scrolling inside the chat.
- Automatic rounding to a supported delivery duration; above 2400 hours, the platform maximum is used.
- Optional follow-up chat after confirmed automatic offers: reuse the request conversation or ask Eldorado to open it, then send separate Solo/Duo text and up to two prepared images per game. Unwritable chats are skipped; uncertain opening/delivery is not automatically retried. Keep AutoOffer open for follow-up dispatch. Real customer chat delivery remains a manual validation.
- Request previews that never submit an offer.
- Clear skip reasons with shortcuts to the relevant settings.
- Automatic settings saves, optional notifications and subscription reminders.
- Optional Eldorado inbox for manual replies.

Eldorado credentials and pricing are stored on your device. Saved Eldorado login uses Windows DPAPI. The subscription service stores AutoOffer account and license information plus a one-way seller-binding fingerprint and short reference. Your Eldorado Client Secret stays on your device.

The bot requires an active subscription, valid Eldorado Seller API access, an internet connection and a running device. New request checks use your configured 1–300 second interval; Eldorado response time also affects delivery of an offer. Closing the app stops the bot unless you choose to minimize it to the tray.

Early builds are unsigned. SHA-256 checksums accompany published downloads. This repository distributes downloads and documentation; the application and subscription-service source are not published here.

---

## بالعربي

حمّل النسخة المناسبة من **Releases**. نسخة Setup للتثبيت، وPortable للتشغيل المحمول. مش محتاج تثبّت Node.js.

سجّل دخولك بالحساب الذي استلمته من الأدمن، ثم اربط حساب Eldorado، وحدد أسعارك ومددك ورسائلك. اعمل فحص الجاهزية قبل تشغيل العروض الحقيقية. الدفع والتجديد خارج البرنامج عن طريق الأدمن.

المعاينة لا ترسل عروضًا. الخانات غير المسعّرة والطلبات خارج فلاترك يتم تخطيها بسبب ظاهر في سجل النشاط. تغيير الأسعار أثناء عمل البوت يُحفظ، لكنه يحتاج إيقاف البوت وتشغيله ليُطبَّق على الإرسال.

الإصدارات الأولى غير موقّعة رقميًا. حسابات العملاء وبيانات Eldorado ومفاتيح إدارة الخدمة لا تُنشر في هذا المستودع.

حساب العميل مرتبط بحساب Eldorado واحد ثابت. فصل الحساب أو إعادة تثبيت البرنامج لا يلغي الربط؛ التغيير من صلاحية الأدمن فقط. تسجيل الدخول من نسخة أخرى ينهي الجلسة السابقة عند التحقق التالي.


للتحديث من 1.0.0: حمّل نسخة Setup الجديدة وثبّتها مرة واحدة. بعدها التحديثات القادمة تُنزّل من داخل البرنامج، والتثبيت بعد إيقاف البوت وحفظ الإعدادات. من الإعدادات العامة تقدر تعمل استيراد وتصدير لأسعارك وفلاترك ورسائلك؛ النسخة الاحتياطية لا تحتوي على الباسوردات أو مفاتيح Eldorado.
