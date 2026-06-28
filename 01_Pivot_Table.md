-- Pivot Table 

-- ye excel ka ek bahut important and powerful tool hai 
Agar hamare pass ek large data hai and us data ko agar hume Summarize krna hai  and uski Proper  report banake in graphical view  hume submit krna hai ya kisi ko dikhana hai to ye kaam hum bahut easily kr skte hai by the help of pivot table 

-- Pahele pure data ko select kro then
Insert-> Pivot table 
New Worksheet pr kholo 

-- Phir sabse pahele hume saara column dikhega jitne bhi hamare table ya excel me the 

-- let say hamari table me employee id,date,Salesman,Product,Qty,Department,State,Sales itni tables hai 

pivot table me 4options dikhte hai 

1) Filter
2) columns
3) Rows 
4) Values-> yha pr hum calculation lagate hai like sum,product etc.

Q-> Let say humse kisi ne kaha ki batao Kis Department me kitni Sale hui hai ye kaam hum badi aasani se pivot table ki madad se kar skte hai

-- hume bss 2 Column se hi matlab hai sales and Department 

-- question me nola gaya hai ki har department ki total sales batao matalab sales ko sum krna hai har department ka 

--So Rows me Department ko daalo and Values me Sales ko daalo i.e show hoga sum of sales 

-- ROWS me department daaloge to row ki form me data dikhega and agar columns me department daaloge to Column ki form me data dikhega 

TRICK-> Agar hum let say electronics pr double tap krtre hai to wo electronic ki saari sale dikha dega ki kis bande ne kb kya electronics item purchase kiya tha 

--hatana hai to select kr ke upar kr do 

--jab hum pivot table bana lete hai to side se pivot wala option hat jata hai matlab row,column,value wala to ye rhe iske liye table select kro the upar Analyze Pivot table then Field list 
Analyze Pivot Table-> Field List 


--Let say humne Department ko utha kr Filter me daal diya isse hoga ye ki ab department pe lag gya hai filter yaani choose kro like kis department ka data dekhna hai i.e Bags,Electronics etc.


Q2 -> Sales State wise dekhna hai with name of customers 

Column-> State and Salesman 
Rows-> Sum of sales 

        OR 

Filter-> State 
Values-> Sum of Sales 
Rows-> Salesman 


Q3-> Kon kon se product beche and kitni Quantity and kon se State me 
    
Rows -> Product 
Filter-> Product and Quantity  
Values-> Sum of Sales

-- Agar hume data aur acche design me chahiye to simply go to Design and report Layout and then Show in Outline Forms 
Design-> Report Layout -> Outline Forms 
isse section divide ho jayega 


-- Kai baar hume Total wala kai baar dikhta hai to use shi krne ke liye 

Subtotal-> Do not show Subtotal 

-- Aur accche form me data dekhna hai to Design-> Report Layout -> Show in Tabular Form  


-- Sab Kuch ek baar me hi delete krna hai to Analyze-> clear-> Clear All

-- Represent data in Percentage 
lets say hume sales ko percentage me show krna hai to 

let say hamari jo total sale hui hai usme hume ye dekhna hai ki har item ka kitna percent contribution hai 

Column-> Product
Value-> Sum of sales
Filter-> Department

iske baad sum of sales me jo value hai usme kisi par bhi right click kro then Sho value as % of grand total 

Show Value AS -> % of Grand Total i.e Grand total ke basis par hume dekhna hai total percentage 

--agar hume iske aage sum of sale dikhana hai to phir se sale ko utha kr value me daal do i.e hum ek hi heading ko kai baar daal skte hai 

-- Handling the missing Values 

Kai baar hamare data me blank values dikti hai use hum handle kr skte hai matlab uski jagah koi bhi value daal skte hai 

table ko select kro -> Right Click->Pivot Table option -> For empty cell show (isme jo value daaloge whi dikhega blank ki jagah like 0,N/A etc.)
phir man ho to data ko align kr do like centre align,left align,right align etc.

-- Q4 Department Wise Product ki sales dikhao 

Rows-> Department and Product
Values-> Sum of sales 

-- Represent Data in Graphical Formate 
 
 kai baar hume data ko graphical form me represent krna hota hai like Graph and Charts ki form me like pie chart,bar graph,scatter plot etc.

 Analyze-> pivot Charts 
 phir design me jake ise customize kr sakte ho 


 -- Slicer 

 Slicer ek tarah ka Visual Filter hota hai matlab filter dikhta hai click krke laga lo

 let say humne ye kiya 

 Column-> department 
 Value-> Sum of Sales 

 Then Analyze-> insert Slicer 
 and select kr lo column ko jispr filter lagana hai like Qty, City etc.

