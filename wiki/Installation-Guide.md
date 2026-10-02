# 📥 คู่มือการติดตั้ง (Installation Guide)

คู่มือนี้แนะนำขั้นตอนการติดตั้ง **Magnus Eterno** ทั้งสำหรับผู้เล่นฝั่ง Client (Java) และผู้ดูแลเซิร์ฟเวอร์ (Server Admin)

---

## 💻 1. การติดตั้งสำหรับผู้เล่น Java (Client)

### ความต้องการของระบบ (Requirements)
- **Minecraft:** Version 26.3
- **Mod Loader:** Fabric Loader (เวอร์ชัน 0.19.5 ขึ้นไป)
- **Java:** Java 25 ขึ้นไป
- **Dependencies ที่จำเป็น:**
  - [Fabric API](https://modrinth.com/mod/fabric-api)
  - [Fabric Language Kotlin](https://modrinth.com/mod/fabric-language-kotlin)

### ขั้นตอนการติดตั้ง
1. ดาวน์โหลดไฟล์ม็อด `magnus-platform-<version>-all.jar` จาก [Modrinth](https://modrinth.com/mod/magnusmod)
2. นำไฟล์ม็อดและ Dependencies ไปวางไว้ที่โฟลเดอร์:
   - **Windows:** `%appdata%\.minecraft\mods`
   - **macOS:** `~/Library/Application Support/minecraft/mods`
   - **Linux:** `~/.minecraft/mods`
3. เปิดตัวเกม Minecraft ผ่านโปรไฟล์ Fabric Loader

---

## 🖥️ 2. การติดตั้งสำหรับผู้ดูแลเซิร์ฟเวอร์ (Dedicated Server)

### Fabric Server Setup
1. ติดตั้ง Fabric Server สำหรับ Minecraft 26.3
2. นำ `magnus-platform-<version>-all.jar`, `fabric-api.jar`, และ `fabric-language-kotlin.jar` ไปไว้ในโฟลเดอร์ `mods/` ของเซิร์ฟเวอร์
3. เริ่มเซิร์ฟเวอร์หนึ่งครั้งเพื่อสร้างไฟล์การตั้งค่าที่ `config/magnusmod.json`

### 📱 การรองรับ Geyser Bedrock (Crossplay)
1. ติดตั้ง **Geyser-Fabric** และ **Floodgate** ในเซิร์ฟเวอร์
2. นำไฟล์ Bedrock Resource Pack `magnus_bedrock_rp.mcpack` ไปวางในโฟลเดอร์ `packs/` ของ Geyser
3. ผู้เล่น Minecraft Bedrock (มือถือ/คอนโซล/Windows 10/11) สามารถเชื่อมต่อเข้ามาเล่นและมองเห็นไอเทมและหน้าต่าง UI ได้ทันที
