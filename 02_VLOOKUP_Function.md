-- VLOOKUP


 ise hum vertical lookup bhi kahte hai ye sirf left se right search karta hai 
 -- let say hamare pass bahut bada data hai and humse manager ya team leader bolta hai ki bhai mujhe empID 102 ki saari details do to aisa nhi hai ki hum line by line search krne baithenge hum simply VLOOKUP ka formula use kr denge 
 --iska use hum tab krte hai jab hume kisi column ke samne uski respective value chahiye kisi column ke base pr
 -- ye first Row return krta hai 


 -- FORMULA of VLOOKUP

=VLOOKUP(lookup_value,table_array,col_index_num,range,range_lookup)



let say hamara data aisa hai 

EmpId     date        Salesman      Product 

1001      1/9/2022     Rajesh       Computer
1002      2/9/2022     Mahesh       Monitor 
1003      3/9/2022     Suresh       Shirt



 -- let say hume us salesman ka naam chahiye jiska EmpID 1002 hai


 -- V.V.V.I-> to VLOOKUP sbse pahele empid me se 1002 dudhenga jaise hi 1002 mila ye usi row me sidha chla jayega and salesman ka naam de dega i.e left to right


1) lookup_value-> Hum kiske adhaar pr data search kr rhe hai i.e EmployeeID jo ki 1002 hai because hume 102 ka hi naam chahiye 
2) table_array-> matlab pra data jis excel file me hai uski puri range 
3) col_index_num-> it means hum jo salesman ka naam dudh rhe hai uska column number kya hai
4) range-> isme hum mostly 0/False likte hai 
agar hume exact match chahyie to likho 0 or False 
agar hume exact match nhi chahiye to likho 1 or True 

so iske according hamara lookup_value=1002,table_array=A2:H14,col_index_num=3(salesman 3 column me hai ),range=o
=VLOOKUP(1002,A2:H14,3,0)


-- agar hum chahte hai ki hume ye A2:H14 na likhna pade to iska ek trick hai 
Pure Table ko selexct kro and upar namebox me isko koi namm de do let say humne naam diya mydata and ab ye likho
=VLOOKUP(1002,mydata,3,0)


-- let say hum yha pr salesman ka naam chahte the to humne likha 3 but iss chiz ko bhi hum automate krna chahte hai 
to iske liye ek formula hota hai Match 
hamare excel ki length A:H hai and salesman C me hai 

=Match(C1,A1:H1,0) ye likh ke enter maaroge to 3 dikhega 

-- let say hum chahte hai ki hum kisi employee ka employeeID daale to usse related uski saari information hume mil jaye 

=VLOOKUP(A2,mydata,MATCH(C1,A1:N1)0) and isme C1 to sbke liye badlega matlab salesman ke liye C1, product ke liye D1.... to ise chod do baaki A1 and N1 ko dekho ye fix rhega because ye range hai 
A1 ab A and 1 ke beech me f4 key press kr do to ye aisa ho jayega $A$1 and similary ye kaam kro N1 ke liye and A2 ke liye bss phir Enter now naam aayega use row me hi N1 tak drag kr do bss
ye c1 se data dega pura end tak drag krne par

VLOOKUP-> Vertical Table

