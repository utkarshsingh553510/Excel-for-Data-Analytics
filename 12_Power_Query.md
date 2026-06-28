-- POWER QUERY 



-- POWER QUERY ek ETL Tool hai matlab

1) E(Extract) -> Data Alag alag source se lana like Csv,Sql,Web,Excwl etc.

2) T(Transform) -> Data ko saaf krna,formate badalana, Duplicates hatana,merge krna etc.

3) L(Load) -> Clean Data ko Excel ya Power BI me Load krna


-- So Power query ek data cleaning and Data Transormation Tool hai let say agar Excel me koi Data gadbad hai like - Extra Spaces,Duplicates Rows,Null Value, Galat Formate etc. to ye sab kaam hum Power Query se kar Skte hai Bina Formula Likhe 


Power Query kya kya kr skta hai 

1) Duplicates hatana 

2) Blank Rows Hatana 

3) Extra Spaces Hatana 

4) Upper/Lower/Proper Case krna

5) Columns Split/Merge Krna 

6) Date Formate badalna 

7) Multiple CSV Files ko Merge/Append krna 

8) Filter and Sort krna 

9) Pivot/Unpivot krna 

10) Data Type Badalna 

11) Refresh krke Naya Data apne aap Update krna 

-- ye free me Microsoft ne diya hai like in Excel,Power BI etc. in sbme hai 


-- Excel me Upar dekhoge to ek DATA krke ek Tab hoga whi Power Query hai 

Home Tab hai phir Insert Tab  .... then Data Tab 

Data Source-> Power Query -> Power Pivot 


Sbse pahele hamare pass Data Source hoga yaani raw data hoga use hum power query ki madad se clean krenge and jab wo clean ho jayega to use hum power Pivot ki madad se Summarize krenge and Charts,Graphs, power Map ki madad se represent krenge 

POWER QUERY me M Language ka Use  Hota hai 
POWER PIVOT me DAX Langugae ka use hota hai



HOW TO USE POWER QUERY ---

1) Sbse pahle Data pr jao and left side Get Data pr click kro and jo data hai use select kro csv me hai ,xlxs me hai etc. use select kro and then click Transform Data 

Data -> Get Data -> Select Data -> Transform Data 


V.V.V.I -> let say hamare pass ek folder hai kai Files hai to agar hum Pure Folder ko select krte hai and clean  krte hai to automatically us Folder ke andar jitne bhi Files hai wo sab automatically Clean Ho jayega 


-- let say hamare pass Ek Csv File hai i.e Marketing Data hai 


 STEP 1) Cleaning messy data: Removing blanks and double headers



Hamare Marketing Data me Double Header hai hum use hatana chahte hai and Bahut sara Cell Khali hai hume use bharana hoga 

Data -> Get Data -> Select Data -> Transform Data 

- Apna marketing ka data select kro and Tranform Data pr click kro 

-- RHS hum dekhenge to payenge ki Applied  Steps yaani abhi tak humne kon kon se Steps Apply kiya hai and let say koi step galat ho jaye to use hum delete ya edit bhi kr skte hai 

-- Navigation pr click krke hum Dusari File Bhi add kr skte  hai isme 


- 1)  Hamare table me Double Header tha so remove it 

Remove Rows -> Remove Top Rows -> Select kro kitne ROws Hatane hai i.e 4

Now Click on Use First Row as Header


2) Har Row Ke Column Name Ke bagal me 123 or ABC likha hota hai jo ki uska data Type Batata hai so Check kro sb Column ka ki sb follow kr rhe hai ya nhi agar Haa to Ok Warna Click kro 123/ABC pr and data type select kro


3) Ab let say hume ye Dekhna hai ki Kisi Column me Kine Empty Cell hai ya Error hai to 

View -> Column Quality 

Valid -> It means Data Sahi hai No Problem 
Error -> It means Data Type Galat hai ya Convert Nhi ho paya 
Empty -> It means ki Cell Empty hai Null hai  

4) Remove Blank Rows 

Home -> Remove Rows -> Remove Blank Rows 

isko krne ke baad 1 column ka pura empty data hat gaya but hume sbka krna hai to 

Ek Column pr Click kro and then ctrl dabao phir second column click kro aise hi kro to saare column select ho jayenge and then kisi bhi column ke header pr click kro Then Mouse Pr LEft click Then Fill Then Down

Select Columns -> Left Click On Column Header -> Fill -> Down 

Agar hume koi value Manually Fill krna hai to Kisi Cell pr click kro then Replace Value 

jb Valid 100% ho jaye tab Ok 


5) Upper/Lower/Proper 

Let say hamara ek Column hai Comapign Name usme Ek column hai The Pinkman promotion  isme promotion me p small letter me hai ise hume uppercase krna hai 

Select Column -> Transform -> Formate -> Capitalize Each Word 


Hum Upper, Lower ,Trim sab kr skate hai 


5) Adding a New Column 

let say hum ek naya column add krna chahte hai jo ki Click / Unit sold kre to simply inn dono columns ko select kro Then Add Column -> Standard -> Divide 

Ab Naya Column ban jayega Divide naam se Iss Column pr Double Click krke Rename bhi kr skte ho 

6) Splitting Columns 

Hum chaye to columns ko split bhi kr skte hai 

Home -> Split Columns -> Based on Delimiters / No of Characters / Postion etc.


7) Load Data 

Now jab Sb Clean Ho jaye to data ko Excel me Load kr do 

Home -> close & Load 


8) Ab jab data Load ho jayega Excel me To hume RHS Queries and connection ka ek option dikhega and Uspr likha hoga like 154 rows affcted simply uspr click kroge to phir se Power Query me pahuch jaoge  Cut kr do agar man nhi hai 
phir se kholna hai to Data -> Queries &b Connections 




-- Does New Data Refresh 

-- agar isi Dataset me koi naya data add on ho jata hai jo ki Clean nhi hai to use hume clean krne ki jrurat nhi hai 
Simply Apne Upar jo Clean Table hai uspr kisi bhi Cell pr Right click krke Refresh kr do Baaki niche jo Unclean Hongi wo Shi Ho Jayengi 



-- Pivot Table 


Agar Hume Iss Data ke liye pivot table bhi chahiye to Queries & Connection pr Niche Dataset ka Kuch naam hoga like Compaign Matrices uspr Right Click kro -> Load to -> Pivot Table Report -> Ok 




-- Combine Your Files 

Let say hamare Pass 3 CSV Files hai RubiksCubeSales_2023,RubiksCubeSales_2024,RubiksCubeSales_2025
and hume ise combine krna hai 


1) Sbse pahele hume In 3 Files ko Ek Folder me Save Krna hoga  Windows C me folder Hoga 

2) Blank Workbook kholo Excel me and Click on Data -> Get Data -> From File -> From Folder 

3) Phir Us Folder ko select kro jisme 3 CSV Files hai and Open and agar Data Clean nhi hai to Combine -> Combine & Transform and Agar Clean hai to Combine -> Combine & Load To Then Ok 

4) kai Baar Hota ye hai ki hamare pass alag alag type ki files hoti hai like Xlxs etc to Power Query Unko Bhi add krne ki koshis krega and If we want ki bss CSV Files hi add on ho to simply click on Source -> Extension -> Click on CSV -> Filter -> Ends With -> Insert -> csv 

Then Combine Hone ke Baad Close & Load to -> Pivot Table bana sakte ho 


5) Nayi Koi File bhi add krte ho to Add Krne ke baad bs Refresh Kr dena 




-- Turn Reports Into Usable Data 

let say Hamare Pass ek Data hai Coffee Unit Sold and ye Bahut Gadbad hai ise Hume Shi krna hai 


1) Coffee Sales ko excel me Kholo 

2) Use pure sheet ko ek Naam do salesCoffee 

3) Phir Get Data ke bagal me Sidhe sidhe 3 File dikhengi 

4) Sbse last wali select kro i.e From Table/Range 

5) Remove Changed Type 

6) Phir 1st Column pr Right Click kro and Unpivot Other Columns 

7) Phir Columns ko naam de do 
1st Column -> Coffee
2nd Column -> Date
3rd Column -> Units Sold 

8) Date Column ko Select kro -> Tranform -> Formate -> Add Suffix -> 2025 
isse Month ke last me 2025 lag jayega ab jab iska datatype date set kroge to last ye year i.e 2025 Dikhega 

8) Har Column ka Datatype set kr dena 
1st column -> Text
2nd Column -> Date 
3rd Column -> Whole no 

10) Phir man ho to Pivot Table me Load kr skte ho 