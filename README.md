# SettingOut_ConstrPier
โปรแกรมคำนวนพิกัดของเสาเข็มที่ประกอบกันเป็นฐานรากขนาดใหญ่ โปรแกรม "Setting_Columns.py" จะอ่านไฟล์ข้อมูล 01_Pier_Schedule.csv แนวตำแหน่งกึ่งกลางของฐานรากและชนิดรูปแบบของฐานรากที่ระบุตำแหน่งของเข็มรับน้ำหนักจำนวนมากกว่าหรือเท่ากับ 1 ต้น จาก  02_CHOS_Pier.yaml โดยระบบ chainage และ offset จากนั้นโปรแกรมจะคำนวนพิกัดของเข็มแต่ละต้น ผลลัพธ์ที่ได้จะมี 2 รูปแบบคือ ไฟล์ข้อมูล GIS ชื่อ 03_PierColumn.gpkg (Geopackage GIS file) ที่สามารถเปิดดูด้วยซอฟต์แวร์ GIS เช่น QGIS เพื่อตรวจสอบความถูกต้องของตำแหน่งและการวางตัวโดยการซ้อนทับกับ แผนที่ภาพดาวเทียม google map  และยังสามารถผลิตพิกัดของเข็มในรูปแบบ CSV ตามต้องการ เพื่อนำไปโหลดเข้า TotalStation หรือ GNSS RTK สำหรับการกำหนดพิกัดในสนาม (Field Setting-out) ต่อไป
ขอขอบคุณ คุณ SubenMukem@ITD ที่เอื้อเฟื้อตัวอย่างข้อมูลและเสนอแนวคิดริเริ่มนำไพธอนมาเขียนสคริปส์ช่วยการคำนวนพิกัดของเสาเข็มที่ประกอบกันเป็นฐานรากขนาดใหญ่นี้

Calculate setting-out coordinates of columns (pile) composing a pier foundation. "Setting_Columns.py" reads 01_Pier_Schedule.csv and 02_CHOS_Pier.yaml file and produce 03_PierColumn.gpkg and 04_Export_Pile_Schedule.csv. A pier could contains many columns specified by local coordinate system and defined in YAML 02_CHOS_Pier.yaml file. The result 03_PierColumn.gpkg (Geopackage GIS file) can be plotted and visualized on GIS software e.g. QGIS.

Acknowledgement: thanks Khun SubenMukem@ITD for sample data and inspiration.

![alt text](https://github.com/phisan-chula/SettingOut_ConstrPier/blob/main/Plot_PierColumns.jpg?raw=True)
