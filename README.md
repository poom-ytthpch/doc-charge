# ⚡ DocCharge

DocCharge คือระบบจัดการการชาร์จ (Charging Management System) สำหรับสถานีชาร์จรถยนต์ไฟฟ้า (EV Charger)  
รองรับการเชื่อมต่อกับ Backend ผ่าน WebSocket / OCPP และมีการแยก Service เป็นโมดูลย่อยที่สามารถนำไปใช้งานร่วมกับโปรเจคหลักได้ผ่าน **Git Submodule**

---

## 🚀 Features

- รองรับการใช้งานผ่าน **Git Submodule**
- WebSocket Service สำหรับเชื่อมต่อ Charger
- รองรับโปรโตคอล OCPP (ส่วนของ Core Handshake / Heartbeat / Status)
- มีโครงสร้างแยกเป็นโมดูลชัดเจน
- Config ใช้งานง่าย
- สามารถนำไปฝังในระบบใหญ่ (Microservices / Monorepo) ได้ทันที

---

## 📦 Installation

โปรเจคนี้ถูกจัดเก็บแบบ **submodule**  
ให้ใช้คำสั่งด้านล่างในการโหลดโค้ดทั้งหมด:

### 👉 Clone โปรเจคหลัก (ถ้ายังไม่ได้ clone)

```sh
git clone https://github.com/poom-ytthpch/doc-charge

cd doc-charge
```

### โหลด DocCharge submodule

```sh
git submodule update --init --recursive
```

### หรือโหลดทุก submodule ในครั้งเดียว:

```sh
git submodule update --init --recursive --remote
```

### 🔧 Project Structure

```sh
/doc-charge
 ├─ apps/
 │   ├─ auth/
 │   ├─ charger/
 │   ├─ gateway/
 │   └─ wallet/
 ├─ client
 ├─ docker
```
