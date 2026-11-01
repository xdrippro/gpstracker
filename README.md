📍 GPS TRACKER
📦 Paket: com.gpstracker.app
🏷 Versiya: 1.2.0 (3-build)
📱 Android 10 va undan yuqori (Android 17 ga moslangan)
🛠 Kotlin + Jetpack Compose (Material 3)

Telefon joylashuvini Telegram botingizga avtomatik yuborib turadigan ilova.

🆕 1.2.0 DA YANGI
• 📩 SMS zaxira yo'li: internet yo'q bo'lsa joy SMS bilan yuboriladi
• 🔎 "JOY XXXX" SMS buyrug'i: telefon yo'qolsa joyni darhol so'rash
• ⚠️ Noto'g'ri joydan himoya (soxta/eski/sakragan joylarni belgilaydi)
• ⚙️ Sozlamalar 2 bo'limli: 1-usul Telegram, 2-usul SMS

▶️ ASOSIY
• Ism kiritish, START va STOP tugmalari
• START bosilishi bilan joy darhol yuboriladi, keyin taxminan har 1 soatda
• Ekran o'chiq bo'lsa ham ishlaydi: Foreground Service va doimiy bildirishnoma ("GPS Tracker Faol", oxirgi tekshiruv vaqti bilan)
• Telefon qayta yoqilganda va ilova yangilanganda kuzatuv o'zi tiklanadi
• Aniq soatli ishga tushirish (Doze rejimida ham)
• Watchdog: har 15 daqiqada xizmatni tekshiradi, o'lgan bo'lsa qayta ishga tushiradi
• Uzilish aniqlansa (95 daqiqadan oshsa) Telegram'ga "Kuzatuv ... davomida uzilgan edi" xabari boradi
• Batareya/Autostart sozlamalariga tez o'tish tugmasi (Oppo, Vivo, Xiaomi va boshqalar)

📨 TELEGRAM XABARI
• Ism, vaqt, kenglik, uzunlik, aniqlik (metr), tezlik (km/soat)
• Batareya foizi va quvvatlanish holati
• Tarmoq turi (Wi-Fi / Mobil internet)
• Google Maps havolasi
• "Ishga tushirildi" va "Hisoboti" xabarlari alohida sarlavhali
• Kechikib yuborilganlari ⏳ belgisi bilan, 25 tagacha nuqta bitta jamlangan xabarda

🔋 TEJAMKOR REJIM
• Joy 30 metrdan kam o'zgarsa nuqta yuborilmaydi
• Joyida turganda ham har 3 soatda "tirikman" nuqtasi boradi
• Joy topilmasa 5 daqiqadan keyin qayta uriniladi, 3 marta ketma-ket topilmasa Telegram'ga ogohlantirish yuboriladi

🌐 INTERNET YO'Q BO'LSA
• Nuqtalar telefon ichidagi navbatga yoziladi (5000 tagacha, 7 kun saqlanadi)
• Internet qaytganda avtomatik yuboriladi, xato bo'lsa qayta urinish kechikish bilan o'sib boradi
• Navbat faqat Telegram "ok" javobi kelgandagina tozalanadi
• Telegram tezlik chegarasiga rioya qilinadi

📩 SMS ZAXIRA (2-USUL)
• Internet yo'q yoki Telegram ishlamasa, eng oxirgi nuqta SMS bo'lib ketadi: ism, sana-vaqt, havola
• Tejash: 30 daqiqada ko'pi bilan 1 ta SMS
• Har SMS'da telefonda bildirishnoma chiqadi (yashirin emas)

🔎 SMS BUYRUQ: "JOY XXXX"
• Saqlangan raqamdan "JOY" va maxfiy kodni yozsangiz, telefon joyni aniqlab o'sha raqamga SMS qiladi, internet bo'lsa Telegram'ga ham yuboradi
• Boshqa raqamdan kelgan buyruqqa javob berilmaydi
• 3 marta xato kod: 1 soat bloklanadi
• 5 daqiqada ko'pi bilan 1 ta javob
• Maxfiy kod ilova PIN'idan alohida
• Har buyruqda telefonda bildirishnoma chiqadi

⚠️ NOTO'G'RI JOYDAN HIMOYA
• 5 daqiqadan eski (keshdagi) joy yuborilmaydi
• Soxta joylashuv (Mock location) aniqlansa belgilanadi
• Aniqlik 100 metrdan yomon bo'lsa belgilanadi
• Oldingi joydan 1200 km/soatdan tez "sakrash" belgilanadi
• Xabarga "⚠️ Diqqat" qatori qo'shiladi

🔐 XAVFSIZLIK
• Ilovaga kirish 4 xonali PIN bilan, PIN sozlamalardan o'zgartiriladi
• PIN o'zi saqlanmaydi: tasodifiy tuz bilan PBKDF2-HMAC-SHA256 (100 000 takror)
• 5 marta xato PIN: 30 soniya qulf, keyin ikki baravar uzayadi (15 daqiqagacha)
• 60 soniyadan uzoq fonda tursa, qaytganda yana PIN so'raladi
• Bildirishnomadagi "To'xtatish" tugmasi ham PIN so'raydi
• Bot Token: Android Keystore, AES-256-GCM bilan shifrlangan
• Koordinatalar bazada shifrlangan
• SMS maxfiy kodi hash holida saqlanadi
• Zaxira nusxa o'chirilgan (bulutga tushmaydi)
• Ilova ma'lumotni faqat Telegram'ga (HTTPS) yuboradi

🔑 RUXSATLAR (bosqichma-bosqich)
• Aniq joylashuv → "Har doim" (fon uchun) → bildirishnoma
• SMS yuborish/qabul qilish: faqat 2-usul yoqilganda

ℹ️ Faqat o'zingiz yoki roziligini bergan odamlarning telefonida ishlating.
