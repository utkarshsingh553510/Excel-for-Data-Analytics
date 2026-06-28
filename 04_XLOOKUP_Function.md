-- XLOOKUP 

XLOOKUP ka matlab hai extended lookup
XLOOKUP = VLOOKUP + HLOOKUP

let say ye ek table hai 

A          B             C            D
EmpId     date        Salesman      Product 

1001      1/9/2022     Rajesh       Computer
1002      2/9/2022     Mahesh       Monitor 
1003      3/9/2022     Suresh       Shirt


ab hume empId 1002 ka naam pata krna hai name C column me hai 

=XLOOKUP(1002,A:A,C:C,0)

xllokup likhne ke baad 1002 likhne ke baad jaha A likha hai uspr click kroge waise hi automatically A:A ho jayega then Similary C pr bhi krna 

-- agar slide krke pura data dekhna hai to simply

=XLOOKUP($A$2,$A:$A,C:C,0) and Drag bss hum A ko fix kr denge because A to employee id hai wo fix hai badlega bss C because C pr Salesman hai then D aayega  to product ho jayega ....

