📍 GPS Tracker (Android, Kotlin)

Telefon joylashuvini Telegram botingizga avtomatik yuborib turadigan ilova. Android 10 va undan yuqori versiyalarda ishlaydi.

⚙️ FUNKSIYALAR

▫️ Ism kiritish maydoni, START va STOP tugmalari
▫️ START bosilishi bilan joylashuv darhol yuboriladi, keyin taxminan har 1 soatda (vaqt bir necha daqiqaga og'ishi mumkin)
▫️ Ekran o'chiq bo'lsa ham ishlaydi: Foreground Service va doimiy bildirishnoma
▫️ Telefon qayta yoqilganda kuzatuv avtomatik tiklanadi (agar yoqilgan bo'lgan bo'lsa)
▫️ Telegram xabarida: ism, vaqt, kenglik, uzunlik, aniqlik (metr), tezlik (km/soat), batareya (quvvatlanish holati bilan), tarmoq turi (Wi-Fi / Mobil internet) va Google Maps havolasi
▫️ Joylashuv topilmasa 5 daqiqadan keyin qayta urinadi, 3 marta ketma-ket topilmasa Telegramga ogohlantirish yuboradi
▫️ Internet bo'lmasa 5 daqiqadan keyin qayta urinadi (6 martagacha)
▫️ Bot Token va Chat ID ilovaning o'zida kiritiladi (⚙️ sozlamalar), token yashirin ko'rinadi
▫️ Ruxsatlar bosqichma-bosqich so'raladi: aniq joylashuv, "Har doim ruxsat" (fon uchun), bildirishnoma
▫️ Ilovaga kirish 4 xonali PIN kod bilan himoyalangan, PIN ni sozlamalardan o'zgartirish mumkin
▫️ Bildirishnomadagi "To'xtatish" tugmasi ham PIN so'raydi
▫️ Zamonaviy Jetpack Compose (Material 3) interfeysi

🔐 MA'LUMOTLAR QANDAY SAQLANADI

🔑 Bot Token: Android Keystore'dagi AES-256-GCM kaliti bilan shifrlab saqlanadi. Kalit Keystore ichida turadi va undan olib bo'lmaydi. Token oddiy matn bo'lib turmaydi, logga yozilmaydi va Intent orqali uzatilmaydi.

🔢 PIN kod: o'zi umuman saqlanmaydi. Faqat tasodifiy "tuz" (16 bayt) bilan PBKDF2-HMAC-SHA256 xeshi (100 000 takrorlash) saqlanadi. Kiritilgan PIN xesh bilan solishtiriladi.

🛡 PIN himoyasi: 5 marta xato kiritilsa 30 soniya qulflanadi, keyingi xatolarda qulf ikki baravar uzayadi (eng ko'pi 15 daqiqa). Ilova 60 soniyadan uzoq fonda tursa, qaytganda yana PIN so'raladi.

👤 Ism va Chat ID: ilovaning shaxsiy xotirasida saqlanadi (boshqa ilovalar o'qiy olmaydi).

☁️ Zaxira nusxa o'chirilgan: ma'lumotlar bulutga yoki ADB zaxirasiga tushmaydi.

🌐 Ilovaning o'zi ma'lumotni faqat Telegramga (api.telegram.org, HTTPS orqali) yuboradi.

⚠️ ESLATMA
• PIN faqat ilova oynasini himoya qiladi, GPS xizmati PIN'dan mustaqil ishlaydi.
• 4 xonali PIN 10 000 ta variantdan iborat. Bu to'liq himoya emas: root huquqli telefonda ilova ma'lumotlarini olish mumkin.
• PIN esdan chiqsa, ilova ma'lumotlarini tozalash kerak, token va Chat ID qayta kiritiladi.
• Faqat o'zingiz yoki roziligini bergan odamlarning telefonida ishlating.
