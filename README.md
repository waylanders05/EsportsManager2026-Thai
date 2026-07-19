# Esports Manager 2026 — มอดภาษาไทย

มอดภาษาไทยสำหรับ **Esports Manager 2026 (Steam / Windows)** แบบ runtime ผ่าน
MelonLoader โดยไม่แก้ไข asset ต้นฉบับของเกม

Repository นี้ใช้สำหรับแจกไฟล์พร้อมเล่นเท่านั้น และไม่มี source code ของมอด

> เวอร์ชันล่าสุด: **v1.0.1**
> ทดสอบกับเกม Steam build `24226509`, Unity `6000.3.12f1` และ MelonLoader `0.7.3`

## ดาวน์โหลดพร้อมเล่น

ดาวน์โหลดไฟล์ `EsportsManager2026.Thai-v1.0.1-Full.zip` จากหน้า
[Releases](../../releases/latest) แพ็กนี้รวม **MelonLoader v0.7.3 x64** จาก
[LavaGang](https://github.com/LavaGang/MelonLoader) ไว้แล้ว ไม่ต้องไปดาวน์โหลดอะไรเพิ่มเอง

วิธีติดตั้ง:

1. ปิดเกม Esports Manager 2026
2. แตก ZIP ออกมาไว้ที่ใดก็ได้
3. ดับเบิลคลิก `Install-ThaiMod.cmd`
4. ตัวติดตั้งจะหา Steam Library และลง MelonLoader กับมอดไทยให้อัตโนมัติ
5. เปิดเกมผ่าน Steam ตามปกติ

หากหาเกมไม่พบ ตัวติดตั้งจะให้เลือกโฟลเดอร์ที่มี `EsportsManager.exe` การเปิดเกม
ครั้งแรกอาจใช้เวลาหลายนาที และ MelonLoader อาจดาวน์โหลด dependency ที่จำเป็น
โดยอัตโนมัติ เพียงเชื่อมต่ออินเทอร์เน็ตไว้ ไม่ต้องติดตั้งด้วยตนเอง

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

หากต้องการถอน MelonLoader ด้วย และไม่มีมอดอื่นใช้งาน ให้ลบ `version.dll` กับโฟลเดอร์
`MelonLoader/` เพิ่มเติม

## แก้ปัญหาเบื้องต้น

- ตรวจว่าเกมปิดอยู่ระหว่างติดตั้งหรืออัปเดตมอด
- แตก ZIP ออกมาก่อน ห้ามเปิดตัวติดตั้งจากภายใน ZIP โดยตรง
- ครั้งแรกให้รอจน MelonLoader สร้างโฟลเดอร์ `MelonLoader/Il2CppAssemblies` เสร็จ
- Log อยู่ที่ `MelonLoader/Latest.log`
- หากเกมอัปเดตแล้วข้อความใหม่ไม่เป็นไทย กรุณาเปิด Issue พร้อมภาพและข้อความจาก log

## ซอฟต์แวร์ที่รวมมา

แพ็กนี้ใช้ไฟล์ทางการ `MelonLoader.x64.zip` รุ่น v0.7.3 โดยไม่ดัดแปลง และตรวจสอบ
SHA-256 ตรงกับ release ของผู้พัฒนา MelonLoader เผยแพร่ภายใต้ Apache License 2.0;
license, notice และ third-party credits ต้นฉบับรวมอยู่ในแพ็กครบถ้วน

## ข้อสงวนสิทธิ์

โปรเจกต์แฟนเมดนี้ไม่มีความเกี่ยวข้องกับหรือการรับรองจาก Neurona Games หรือ Steam
ชื่อเกม เครื่องหมายการค้า และทรัพย์สินของเกมเป็นของเจ้าของที่เกี่ยวข้อง

แพ็กมอดและคำแปลเผยแพร่ภายใต้ [MIT License](LICENSE)
