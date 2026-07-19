# Esports Manager 2026 — มอดภาษาไทย

มอดภาษาไทยสำหรับ **Esports Manager 2026 (Steam / Windows)** แบบ runtime ผ่าน
MelonLoader โดยไม่แก้ไข asset ต้นฉบับของเกม

Repository นี้ใช้สำหรับแจกไฟล์พร้อมเล่นเท่านั้น และไม่มี source code ของมอด

> เวอร์ชันล่าสุด: **v1.0.1**
> ทดสอบกับเกม Steam build `24226509`, Unity `6000.3.12f1` และ MelonLoader `0.7.3`

## ดาวน์โหลดพร้อมเล่น

ดาวน์โหลดไฟล์ `EsportsManager2026.Thai-v1.0.1.zip` จากหน้า
[Releases](../../releases/latest) แล้วแตกไฟล์ลงในโฟลเดอร์เกม เช่น:

```text
E:\SteamLibrary\steamapps\common\Esports Manager 2026
```

หลังแตกไฟล์ควรได้โครงสร้างนี้:

```text
Esports Manager 2026/
└─ Mods/
   ├─ EsportsManager2026.Thai.dll
   └─ EsportsManager2026.Thai/
      └─ th.json
```

ต้องติดตั้ง **MelonLoader 0.7.x (x64)** และเปิดเกมอย่างน้อยหนึ่งครั้งก่อนใช้งาน
จากนั้นเปิดเกมตามปกติ มอดจะใช้ช่อง `sv-SE` ภายในและแสดงชื่อภาษาเป็น `ไทย`

## ขอบเขตคำแปล

- Unity String Tables 4,827 รายการ
- อีเมลและข้อความจำลอง 1,330 รายการ
- บทสนทนา 1,144 รายการ
- Loading tips ครบ 100 ประโยค
- รองรับ SmartFormat, placeholder, rich text และ gender token
- ฟอนต์ไทย TextMeshPro พร้อมชื่อวันและเดือนภาษาไทย

ชื่อทีม ผู้เล่น แบรนด์ รายการแข่งขัน และศัพท์สั้นบางรายการ เช่น `STAGE 2/3`
คงรูปเดิมโดยเจตนา

## ถอนการติดตั้ง

ปิดเกม แล้วลบ:

```text
Mods/EsportsManager2026.Thai.dll
Mods/EsportsManager2026.Thai/
```

หรือใช้ `scripts/uninstall_release.ps1` โดยระบุ `-GameDir` หากเกมไม่ได้ติดตั้งที่ค่าเริ่มต้น

## แก้ปัญหาเบื้องต้น

- ตรวจว่าเกมปิดอยู่ระหว่างติดตั้งหรืออัปเดตมอด
- ตรวจว่า MelonLoader สร้างโฟลเดอร์ `MelonLoader/Il2CppAssemblies` แล้ว
- Log อยู่ที่ `MelonLoader/Latest.log`
- หากเกมอัปเดตแล้วข้อความใหม่ไม่เป็นไทย กรุณาเปิด Issue พร้อมภาพและข้อความจาก log

## ข้อสงวนสิทธิ์

โปรเจกต์แฟนเมดนี้ไม่มีความเกี่ยวข้องกับหรือการรับรองจาก Neurona Games หรือ Steam
ชื่อเกม เครื่องหมายการค้า และทรัพย์สินของเกมเป็นของเจ้าของที่เกี่ยวข้อง

แพ็กมอดและคำแปลเผยแพร่ภายใต้ [MIT License](LICENSE)
