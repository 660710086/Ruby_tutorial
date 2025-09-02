# Instance Variables
**Instance Variables** ในภาษา Ruby คือตัวแปรที่เป็นสมาชิกของ Object แต่ละตัว โดยที่ Instance Varibles ต้องขึ้นต้นด้วยเครื่องหมาย @ ชื่อตัวแปร Instance Variables จะเป็นไปตามกฏ local และเนื่องจาก Instance Variables ขึ้นต้นด้วยเครื่องหมาย @ อักขระตัวที่สองอาจจะเป็นตัวพิมพ์ใหญ่ได้

## 🍅 คุณสมบัติหลักของ Instance Variables มีดังนี้

❀ การประกาศ Instance Variables ในภาษา Ruby ไม่จำเป็นจะต้องประกาศล่วงหน้า เราสามารถสร้างขึ้นแบบ dynamic ได้เมื่อมีการเรียกใช้งานเป็นครั้งแรก  
❀ การเข้าถึง Instance Variables จะเป็นแบบ private ไม่สามารถเข้าถึงจากภายนอก class ได้โดยตรงจะต้องผ่าน methods หรือใช้ attr_reader ,attr_writer ,attr_accessor  
❀ ก่อนที่จะมีการกำหนดค่า Instance Variables จะต้องมีค่าเป็น nill  
❀ Object แต่ละตัวจะมี Instance Variables ที่แตกต่างกันแม้ว่าจะอยู่ใน classเดียวกัน  
❀ ในการตรวจสอบ/แก้ไข สามารถทำได้ด้วย instance_variables ,instance_variable_get ,instance_variable_set ,remove_instance_variable  
## 🍅 ตัวอย่างโค้ด  
### กำหนดและการใช้งาน  
📌 โค้ด  

      ```ruby  
      class Person
      def initialize(name, age)
        @name = name
        @age = age
      end

      def info
        "ชื่อ: #{@name}, อายุ: #{@age}"
      end
    end
    
    a = Person.new("นิว", 25)
    b = Person.new("ใหม่", 30)

    puts a.info
    puts b.info  
    ```  

📌 ผลลัพธ์
☞  อันนี้แสดงให้เห็นได้ว่าแต่ละออบเจ็กต์จะมี instance variable เป็นของตัวเอง[4]  
### ค่าเริ่มต้น  
📌 โค้ด  
    

    
  

  
# Reference 
https://ruby-doc.org/docs/ruby-doc-bundle/UsersGuide/rg/instancevars.html นำเนื้อหาคุณสมบัติของ Instance Variables มาใช้ สืบค้นเมื่อวันที่ 1 กันยายน 2568  
https://docs.ruby-lang.org/en/3.3/syntax/assignment_rdoc.html  นำเนื้อหาเรื่องInstance Variablesเรื่องกฎการตั้งชื่อมาใช้ สืบค้นเมื่อวันที่ 1 กันยายน 2568  
https://ruby-doc.org/core/Module.html?utm_source=chatgpt.com Ruby Core API – Module#attr_reader, Module#attr_writer, Module#attr_accessor.  
https://ruby-doc.org/3.4.1/Object.html?utm_source=chatgpt.com Ruby Core API – Object#instance_variables, #instance_variable_get, #instance_variable_set, #remove_instance_variable.  
[4]https://www.tutorialspoint.com/ruby/ruby_variables.htm?utm_source=chatgpt.com  TutorialsPoint – Ruby Variables.



