-- TEXT FUNCTIONS 


ye wo functions hote hai jo ki text ko manipulate ya Clean krte hai 


1) LEN()

- Ye Hume batata hai ki Text me kitne Characters hai 

let say hume batana hai ki kisi Employee ka naam kitne charaters ka hai and Let say employee name B column me hai 

=LEN(B2)



2) LEFT 

=LEFT(B2,4)

- ye B2 me jo employee hai uske naam ka pahela 4 character dega i.e Left se 


3) RIGHT

=RIGHT(B2,4)

- ye B2 me jo employee hai uske naam ka last 4 character dega i.e right se 


4) MID 

=MID(B2,3,5)

-- let say B2 employee ka naam Bholu Singh hai then ye 3rd character se count krega next 5 characters including #rd character and space  

O/P-> olu S



5) UPPER()

-Ye sbko Capital kr dega 

=UPPER(B2)



5) LOWER()

-Ye sbko Small kr dega 

=LOWER(B2)



6) PROPER()

- ye Har Word ka First letter Capital Kr dega 

=PROPER(B2)

like amit singh hai use ye Amit Singh kr dega 



7) TRIM()

- Ye extra Spaces Remove kr deta hai 

=TRIM(B2)

Like Amit   Singh   ko ye simply Amit Singh kr dega 


8) CONCAT()

-- Ye basically do Text ya Strings ko aapas me Jod deta hai 

Let say Department and Gender ko Jod do 

=CONCAT(C2,"-",D2)

- let say C2 me tha HR and D2 me tha Male 
O/P-> HR-Male


10) TEXT()

-- ye Basically numerical data ko text data me convert kr dega 

let say hamare pass date hai ek 01-07-2026 and hume ise dd-mm-yyyy formate me krna hai 
 and ye Date let say F column me hai 

 =TEXT(F2,"dd-mm-yyyy")


11) REPT()

- kisi value ko hume jab repeat krwana hota hai to hum iska use krte hai 

=REPT(E2,4)

--ye E2 me jo value hai use 4 Times Repeat kr dega 

12) FIND() and SEARCH()

-- In dono ka kaam hai kisi text ko search krna and uska indecx number batana 
-- FIND case Sensitive hai 
-- SEARCH case Sensitive nhi hai 

=FIND("y",D5)

= SEARCH("y",D5)



13) SUBSTITUE()

Q1) Department me jaha jaha HR hai use Replace Karo Human Resource se 

=SUBSTITUTE(D2,"HR","Human Resource")



14) VALUE()

Ye Text ko Number me Convert krta hai 

let say E column me Salary hai 

=VALUE(E2)
