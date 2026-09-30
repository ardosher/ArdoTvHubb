# ArdoTv Hub

Artel (Android TV) televizorlari uchun ilovalar markazi. Pult bilan boshqariladi.

## APK ni GitHub'da yig'ish
1. github.com da yangi repozitoriy oching (masalan `ArdoTvHub`).
2. Shu papkadagi hamma fayllarni (`.github` papkasi bilan) repozitoriyga yuklang.
3. Repozitoriyda **Actions** bo'limiga kiring. "APK yig'ish" ishga tushadi (2-5 daqiqa).
4. Tugagach, ish sahifasi pastidagi **Artifacts** dan `ArdoTvHub-apk` ni yuklab oling (zip ichida `app-debug.apk`).
5. APK ni Telegram orqali yuboring, televizorda yuklab olib o'rnating (Sozlamalar > Xavfsizlik > Noma'lum manbalar).

## Ilova qo'shish/olib tashlash
`app/src/main/assets/apps.json` faylini tahrirlang:
- `name`: kartochkadagi nom
- `packages`: ilovaning paket nomi (bir nechta variant yozish mumkin)
- `color`: kartochka rangi
- `url` (ixtiyoriy): ilova o'rnatilmagan bo'lsa ochiladigan havola (masalan APK yuklash sahifasi)

Paket nomi bo'sh qoldirilsa, o'rnatilmagan holatda Play Market'da nom bo'yicha qidiriladi.

## Qo'shimcha imkoniyatlar
- **Oxirgi ochilganlar**: eng ko'p ochilgan ilovalar tepada chiqadi.
- **Kirishlar (HDMI)**: televizor HDMI kirishlari kartochka bo'lib chiqadi (televizor qo'llab-quvvatlasa).
- **Barcha ilovalar**: televizorda o'rnatilgan hamma ilova avtomatik ko'rinadi.
- **Launcher rejimi**: Home tugmasi bosilganda "ArdoTv Hub" ni tanlab, "Doim" ni bossangiz, televizor yoqilganda shu ilova ochiladi. Eski holatga qaytarish: Sozlamalar > Ilovalar > ArdoTv Hub > "Standart sozlamalarni tozalash".
