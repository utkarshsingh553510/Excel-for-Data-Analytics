-- LOGICAL FUNCTIONS 

ye wo functions hote hai jo ki conditions ko check krte hai and uss condition ke according decision lete hai 
like-> Agar age>18 then Driving Licence milega warna nhi

> -> Greater Than 
< -> Less Than 
>= -> Greater Than or Equal to
<= -> Less Than or Equal to
= -> Equals To
<> -> Not Equals To

1) IF Function 

Syntax-> (Condition,value_if_true,value_if_false) 

agar condition true hai to value_if_true chlega nhi to value_if_false chlega 

Q1) let say hume ek condition lagani hai agar salary 40K se jyada hai to bonus 30% , agar salary 30 k se km hai to 20% bonus ,and agar salary 20k se kam hai to 10% bonus 
let say salary column E me hai

=IF(E2>40000,E2*30%,IF(E2<30000,E2*20%,IF(E2<20000,E2*10%)))
Now Drag kro sbka Bonus nikal jayega 


-- Q2) let say agar student 50 ya 50 se jyada marks paaya hai to pass nhi to fail

=IF(E2>=50,"PASS","FAIL")

-- let say humne likha =E2=E4 agar value same hai to True return hoga warna false 


2) OR  FUNCTION -> Agar ek bhi condition true hai to ye true return krega warna false 

let say humne likha

=OR(E2=E30,E3>E27) Agar isme se ek bhi condition true hogi to ye true return krega 

-- Q1) agar salary 25000 se jyada hai ya gender male hai tabhi increment hoga 

--Formula me column ka naam nhi likhte hai uski cell value daalte hai 

=OR(E2>25000,C2="male")


3) AND FUNCTION -> agar dono condition true hai tabhi ye true dega warna false


--Q1) agar salary 25000 se jyada hai and gender male hai tabhi increment milega 

=AND(E2>25000,C2="male")


--Q2) agar salary 25000 se jyada hai and gender male hai and department Sales hai tabhi increment milega 

=OR(E2>25000,C2="male",D2<>"Sales")


4) IF + OR FUNCTION

-- Q1) let say humse kaha gya ki agar salary 30 k se jyada hai ya department HR hai tabhi bonus do 20% ka warna No bonus 

=IF(OR(E2>30000,D2<>"HR"),E2*20%,"NO BONUS")
sbka dekhna hai to drag kr dena enter maarne ke baad 


5) IF + AND FUNCTION 

-- Q1) let say humse kaha gya ki agar salary 30 k se jyada hai and department HR hai tabhi bonus do 20% ka warna No bonus

=IF(AND(E2>30000,D2<>"HR"),E2*20%,"NO BONUS")
sbka dekhna hai to drag kr dena enter maarne ke baad 


6) IF ERROR 

iska use error ko chupane ke liye kiya jata hai ki agar hamare table me error aa gya to uski jagah kya show kroge 

-- Syntax

=IFERROR(value,value_if_error)

-- Q1) let say hamare table me humne kiya 0/2 to ye to error show krega and hum chahate hai ki ye OK show kre 
let say 0 E2 me hai and 2 F2me hai 

=IFERROR(E2/F2,"OK")

7) IFS 

iska use multiple conditions ko check krne ke liye hota hai 

--Q1) let say jo employee 40000 se jyada salary pa rhe hai unke pr likho very high , jo 30000 se kam pa rhe hai unke pr likho Medium ,and jo 20000 se kam pa rhe hai unke pr likho Low 
let say salary E column me hai 

=IFS(E2>40000,"Very High",E2<30000,"Medium",E2<20000,"Low")


8) SUMIF 

ye ek condition ke basis pr values ko add krta hai 

Syntax->  =SUMIF(range,criteria,sum_range)

Q1)  let say hume ye pata krna hai ki HR department me jitne log hai un sbki salary kitni hai 

-- let say department D column me hai and Salary E column me hai 
-- sbki range 1 to 51 hai 

= SUMIF(D2:D51,"HR",E2:E51)

-- ye HR dpartment me jitne log hai un sbki salary nikal kr add krke  final output de dega 

-- Isme bss problem ye hai ki yha hum bss ek hi condition de skte hai 



9) SUMIFS 

-- yha par hum multiple conditions de sakte hai 

--Q1) Aise employee ka data batao Jo ki HR department ka hai and salary 40000 se jyada hai 

=SUMIFS(E2:E51,D2:D51,"HR",E2:E51,">40000")



-- Q2) Let say hume ye batana hai ki sales department me se aise employee ka salary ka sum nikalo jinki salary 250000 se jyada hai and gender male ho 

Salary niakla hai pahele i.e Column E
Department hai Sales i.e Column D
Gender column C me hai

=SUMIFS(E2:E51,D2:D51,"Sales",C2:C51,"Male",E2:E51>"25000")



10) NOT 
 
 - ye true ko false and false ko true batata hai 

 =NOT(E4>E12)

 let say E4 bada hai to  Not(true)-> False  ye output aayega 



