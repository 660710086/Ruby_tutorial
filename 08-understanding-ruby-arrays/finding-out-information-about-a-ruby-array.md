# 📘 Finding Out Information about a Ruby Array

ในภาษา **Ruby** มีเมธอด (methods) และคำสั่งมากมายที่สามารถใช้ร่วมกับ **Arrays** ได้  
โดยสามารถแบ่งการใช้งานออกเป็น 5 ประเภทใหญ่ ๆ ดังนี้:  

1. **Access / Retrieval** (การเข้าถึงข้อมูล)  
2. **Query / Information** (ตรวจสอบ / หาข้อมูล)  
3. **Modification / Mutation** (แก้ไขค่าใน Array)  
4. **Enumeration / Iteration** (วน loop / map / filter)  
5. **Advanced / Combinatorics / Utilities** (การใช้งานขั้นสูง / การคำนวณ / สถิติ)

---

## 1. Access / Retrieval (การเข้าถึงข้อมูล)

**ยกตัวอย่างการสร้าง array**
```ruby
arr1 = [1,2,3,4,5,6,7,8,9]
arr2 = [[1,2,3],[4,5,6],[7,8,9]]
```
การเข้าถึง array สามารถทำได้ 2 วิธี คือ
1. การเข้าถึงเเบบปกติ
```ruby
