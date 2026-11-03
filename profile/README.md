# Moby

**Windows kompyuteringiz yonida turadigan ovozli AI yordamchi robot.**

Moby Mini — ESP32-S3 asosidagi ixcham stol roboti. U holatini OLED ekrandagi jonli ko‘zlar orqali ko‘rsatadi. Loyiha maqsadi — tugmani bosib so‘rov aytish va Windows kompyuterida o‘zingiz ruxsat bergan amallarni bajarish. Masalan, Moby siz tanlagan loyihaning Git holatini tekshirishga yordam beradi.

<p align="center">
  <img src="https://raw.githubusercontent.com/mobyuz/3d-model/main/moby-mini-assembled.png" alt="Moby Mini 3D modeli. Old panelda OLED ko‘zlar, mikrofon kaliti va Talk tugmasi ko‘rinadi." width="480">
  <br>
  <em>Moby Mini korpusining Blender renderi</em>
</p>

## Moby qanday ishlashi rejalashtirilgan?

1. **Robot.** Talk tugmasi ovoz qabulini boshlaydi. OLED tinglash, mikrofon o‘chirilgan yoki ulanish uzilgan holatlarni ko‘rsatadi. Jismoniy kalit mikrofonning ma’lumot liniyasini uzadi.
2. **Windows ilovasi.** Robot USB orqali ulanadi. Ilova suhbat tarixini kompyuterda saqlaydi, mahalliy amallar uchun ruxsatlarni tekshiradi va foydalanuvchi ruxsat bergan amallarni bajaradi.
3. **Moby API.** Ovozli so‘rov foydalanuvchi roziligi bilan serverga yuboriladi. Server nutqni matnga aylantirish, AI javobini olish va javobni ovozga aylantirishni boshqaradi.

## Repozitoriylar

| Repozitoriy | Nimalar bor? |
| --- | --- |
| [moby-firmware](https://github.com/mobyuz/moby-firmware) | ESP-IDF va C asosidagi firmware. OLED ifodalari, tugma va mikrofon kaliti holati, mikrofon uchun stend sinovi. |
| [moby-api](https://github.com/mobyuz/moby-api) | Rust, Axum va PostgreSQL asosidagi API. Hisoblar, sessiyalar, rozilik, foydalanish limitlari va OpenAPI kontrakti. AI va ovoz oqimlari uchun sinov javoblari. |
| [moby-web](https://github.com/mobyuz/moby-web) | React, TypeScript va Vite asosidagi tanishtiruv sayti. |
| [3d-model](https://github.com/mobyuz/3d-model) | Moby Mini’ning Blender modellari, komponentlar ro‘yxati va sim ulanishlari. |

## Hozirgi holat

Moby prototip bosqichida. Firmware yig‘ilgan va avtomatlashtirilgan sinovlardan o‘tgan. Mikrofon va boshqaruv elementlarini real platada sinash, shuningdek robot, Windows ilovasi va serverni yagona ovozli oqimga ulash rejalashtirilgan. API’ni Docker Compose orqali, tanishtiruv saytini esa Vite orqali alohida mahalliy ishga tushirish mumkin. Yo‘riqnomalar tegishli repozitoriylarda.
