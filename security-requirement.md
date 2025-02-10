# 🔐 Security Requirement

## 📌 13.1.5 Generic Web Service Security

✅ **ข้อกำหนด:**  
Verify that requests containing unexpected or missing content types are rejected with appropriate headers (HTTP response status 406 Unacceptable or 415 Unsupported Media Type).
---

## 💡 คำแปลจาก AI Model & My Self

| 🤖 **ChatGPT**  | ตรวจสอบให้แน่ใจว่า ระบบปฏิเสธคำขอ (Request) ที่มีประเภทเนื้อหา (Content-Type) ไม่ถูกต้องหรือไม่มีข้อมูลประเภทเนื้อหาตามที่คาดไว้ โดยต้องตอบกลับ (Response) ด้วยสถานะ HTTP ที่เหมาะสม เช่น

406 Unacceptable – เมื่อเซิร์ฟเวอร์ไม่สามารถให้ข้อมูลในรูปแบบที่ผู้ใช้ร้องขอได้
415 Unsupported Media Type – เมื่อเซิร์ฟเวอร์ไม่รองรับประเภทเนื้อหาของคำขอที่ส่งมา
การทำเช่นนี้ช่วยป้องกันข้อผิดพลาดและทำให้ระบบจัดการข้อมูลได้อย่างถูกต้อง✅ |
|---------------|------------------------------------------------------------------------------------------------------------------------------------|
| ✨ **Gemini**  | ตรวจสอบให้แน่ใจว่าคำขอ (requests) ที่มีข้อมูล (content types) ที่ไม่ถูกต้องหรือไม่ครบถ้วน จะถูกปฏิเสธ (rejected) โดยมีรหัสข้อความแสดงความผิดพลาด (HTTP response status) ที่เหมาะสม เช่น 

406 (Unacceptable) หรือ 415 (Unsupported Media Type) ✅ |
| 🧠 **My Self** | ตรวจสอบว่าระบบนี้สามารถปฏิเสธคำขอที่มีประเภทเนื้อหา (Content-Type) ไม่ถูกต้องหรือไม่ได้ระบุประเภทเนื้อหาเลย โดยต้องส่งการตอบกลับ (Response) ด้วยสถานะ HTTP ที่เหมาะสม เช่น

406 Unacceptable – ใช้เมื่อเซิร์ฟเวอร์ไม่สามารถให้ข้อมูลในรูปแบบที่ผู้ร้องขอต้องการ
415 Unsupported Media Type – ใช้เมื่อประเภทเนื้อหาที่ส่งมาไม่รองรับ

พูดง่าย ๆ ก็คือ ระบบต้องสามารถตรวจจับและปฏิเสธคำขอที่ไม่ได้ใช้รูปแบบข้อมูลที่ถูกต้อง พร้อมแจ้งให้ผู้ใช้หรือโปรแกรมที่เรียกใช้งานทราบว่าข้อผิดพลาดเกิดจากอะไร💯 |

---

## 🔗 Link
🔍 **[Security Requirements by TinnapopR](https://tinnapop-1728.github.io/security-requirement)**

