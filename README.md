# SettingOut_ConstrPier
Calculate setting-out coordinates of columns composing a pile foundation. Software reads 01_Pier_Schedule.csv and 02_CHOS_Pier.yaml file and produce 03_PierColumn.gpkg and 04_Export_Pile_Schedule.csv.

A pier could contains many columns specified by local 
        coordinate system  e.g. type F4B-U
                       | Y
                       |
                 3+    |     +2      
                       x (PIER) -------------> X
                 4+          +1 (column number) 
   
