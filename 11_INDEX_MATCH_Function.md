-- INDEX + MATCH 

- ab hum dono ko saath me lenge 

let say hamare Pass ye table hai 

A              B
Name          Salary  

Amit           25000    
Ravi           30000
Neha           35000
Mohan          40000


Q1) Neha Ki Salary Nikalo with the help of index + match 


STEP 1-> Sbase Pahele Match se Neha ki position Nikalo 

=MATCH("Neha",A2:A5,0)

isse hume neha kis postion pr hai uski value mil jayegi i.e 3


STEP 2 -> Ab Index Function use kro and Salary wali column(B2:B5) me se 3rd Value Nikalo 

=INDEX(B2:B5,3)

O/P-> 35000



- Now Index and match dono ko saath me use kro

=INDEX(B2:B5,MATCH("Neha",A2:A5,0))

How it works---

1) Sbase pahle Match function chlega i.e =MATCH("Neha",A2:A5,0) and ye output dega 3

2) Ab Index function chlega and ye ho jayega 
=INDEX(B2:B5,3) and ye ouput de dega 35000 

i.e Neha ki salary pata chal gyi 




Q2) EmpID 116 ki salary nikalo 

let say EmpId A column me hai and salary E column me hai 

=INDEX(E2:E18,MATCH(116,A2:A18,0))


- MATCH(116,A2:A18,0) ye EmpID 116 ki position bata dega let say postion 17 hai 

=INDEX(E2:E18,17)

ye 17 no ki salary de dega 

