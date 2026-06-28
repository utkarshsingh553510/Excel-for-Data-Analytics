-- HLOOKUP 

HLOOKUP matlab hota hai horizontal lookup 
ye horizontal data search karta hai 
ye first column return krta hai 

--V.V.V.I -> let say hamara data aise hai 

EmpID     1001      1002       1003     
date      1/9/2022  2/9/2022   3/9/2022
Salesman   Rajesh    Mahesh    Suresh
Product    Computer  Monitor    Shirt


-- ab let say humne kaha ki hume empId 1002 ka naam batao to ye sbse pahele first row me dekhega ki 1002 kaha hai ye jaise hi mila wo niche jayega and name de dega 

HLOOKUP-> Horizontal Table

Formula iska same hai Vlookup ki tarah hi bss yaha pr Hlookup lag jata hai 

let say hume empId 1002 ka naam chahiye 

= HLOOKUP(1002,A1:H14,3,0)
