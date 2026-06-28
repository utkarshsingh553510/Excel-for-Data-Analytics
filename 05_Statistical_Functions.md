-- STATISTICAL Functions 

1) AVERAGE 

let say hume pure table me salary ka average nikalana hai

salary Column E me  hai and iski range 2 se 51 hai 

=Average(E2:E51)



2) MAX 

- ye table me se max value nikal kr de dega 

=MAX(E2:E51)
 
 let say salary me ye daaloge to ye max salary nikal kr de dega 



3) MIN

- ye min value nikal kr de dega 
- let say hum ye salary table pr ye lagayenge to ye minimum salary nikal dega 

=MIN(E2:E51)



4) COUNT 

- ye total Cell count krta hai 
- ye bss numerical data ko count krta hai ye Text data ko count nhi krta hai  

=COUNT(E2:E51)



5) COUNTA

-- ye text and numerical dono data ko count krta hai

=COUNTA(E2:E51)




6) COUNTBLANK

- ye bss Empty Cell ko count krta hai 


let say hamare salary Column me bss 2 cell empty hai

=COUNTBLANK(E2:E51)

iska output aayega 2 




7) COUNTIF 

- iski madad se hum jo text  baar baar repeat hua hai use count kr skte hai 

- let say hamare gender column me male and female kai baar aaya hai to hume let say ye count krna hai ki male kitni baar aaya hai to hum ye simply kr skte hai countif ki madad se 

let say gender column C me hai 


=COUNTIF(C2:C51,"Male")



8) COUNTIFS

- Ye multiple conditions ke basis pr count krta hai

Q1) let say humse pucha jaye ki Sales department ki kitni female employees hai 

- Department column D me hai and gender column C me hai 

=COUNTIFS(D2:D51,"Sales",C2:C51,"Female")


9) AVERAGEIF

ye ek conditions ke basis pr average nukalta hai


-Q1) HR department ki Average Salary Nikalo

=AVERAGEIF(D2:D51,"HR",E2:E51)


10) AVERAGEIFS 

- ye Multiple Conditions ke basis pr Average nikalata hai 

-Q1) HR Department me Male ki Average Salary Nikalo 

=AVERAGEIFS(E2:E51,D2:D51,"HR",C2:C51,"Male")



11) MEDIAN 

- Ye data ki middle value Nikalata hai 

=MEDIAN(E2:E51)



12) LARGE 

- ye Nth Highest Value nikalata hai


Q1) Find Highest Salary 

=LARGE(E2:E51,1)


Q2) FInd 2nd Highest salary

=LARGE(E2:E51,2)


Q3) Find 3rd Highest salary 

=LARGE(E2:E51,3)




13) SMALL 

-ye Nth Lowest Value batata hai 


Q1) Find lowest Salary 

=SMALL(E2:E51,1)



Q2) Find 2nd lowest salary

=SMALL(E2:E51,2)


14) RANK

SYNTAX-> =RANK(number,Range,0/1)

0-> Ascending
1-> Descending 


let say hume salary ko rank krna hai ki jiski salary sbse jyada use 1 phir usse km to 2....

=RANK(E2,$E$2:$E$51,0)



15) SUM 

ye value ko aapas me add krti hai 

=SUM(E2:E4)



16) MODE 

- ye sbse jyada repeat hone wali value batati hai 

=MODE(E2:E51)



