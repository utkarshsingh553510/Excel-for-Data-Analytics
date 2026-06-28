-- INDEX  FUNCTION 

1) INDEX FUNCTION 

- Ye kisi range me di gayi Row and Column ki Value Return krta hai 

- ye VLOOKUP se jyada Flexible hota hai and Aaj ke Time pr Company Mostly iska Use krti hai

Syntax -> =INDEX(array,row_num,[column_num])

yaha array ka matlab hai range jo aap de rhe ho 


A         B              C        D             E         F
Emp ID	Employee Name	Gender	Department     Salary   Date 
101	Amit Sharma	Male	HR	       25000	1/7/2026
102	Priya Singh	Female	Sales	       18000	1/8/2026
103	Rahul Verma	Male	IT	       42000	1/9/2026
104	Neha Gupta	Female	Finance	       35000	1/10/2026
105	Mohit Kumar	Male	Sales	       22000	1/11/2026
106	Pooja Yadav	Female	HR	       28000	1/12/2026
107	Rohan Mishra	Male	IT	       45000	1/13/2026
108	Anjali Roy	Female	Finance	       38000	1/14/2026
109	Suresh Patel	Male	Sales	       17000	1/15/2026
110	Kavita Jain	Female	HR	       26000	1/16/2026




- COLUMN WISE 


Q1)  Let say D column me Department hai and hume pata krna hai ki 4 no me kon sa department hai 

=INDEX(D1:D10,5)

humne 5 isliye liya hai because ek Row to Department bhi hai i.e 1st yhi hai 



-- ROW WISE 


Q1) let say ye hamari ek table hai and hume EmpId 102 wale ka naam chahiye 

102 A3 me hai and uska naam B3 me hai and B3 2nd column hai 

=INDEX(A3:B3,3)


Q2) Mujhe Empid 103 Ka Gender do 

Gender C column me hai i.e 3rd and 103 A4 me hai

=INDEX(A4:C4,3)    

ya pura row select kr lo no problem 

=INDEX(A4:F4,3)



-- ROW AND COLUMN BOTH 



- Syntax-> =INDEX(array,row_no,col_no)

1) array matalab range jo aap doge 

2) Row_no matlab kis row se value nikalna hai 

3) col_no matlab kis column se value nikalana hai 



Ex-> =INDEX(A1:F51,5,5)

puri table ki range A1:F51 hai ab humne puri table me se 5 row and 5 column liya hai jaha pr inka intersection hoga wo value milegi 



=INDEX(A1:F51,10,3) 

it means 10th row ke  3rd column ki Value do 



-- let say hume pura data nikalna hai kisi row ka 

=INDEX(A1:F51,2,)

ye 2nd Row ka pura data nikal dega 



-- let say hume kisi column ka pura data nikalna hai 

= INDEX(A1:F51,,4)

ye 4th column ka pura data nikal dega 
