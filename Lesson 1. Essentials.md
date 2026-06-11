# 1.1 Setting Up for the Course


first because I am using OnDemand, I must modify the **cre8data.sas** 

```
/*************************************************************
 Note: This program will not run properly on z/OS.
       Only Windows, Linux and UNIX are supported.

 STEP 1: Notice the default values for the %LET statements. 

 STEP 2: If your files will not be located in S:/workshop 
         change the value of PATH= in the %LET statement to 
         reflect your actual data location. 

 STEP 3: Submit the program to create the course data files. 

 STEP 4: Review the SAS log to ensure there are no errors. 

 STEP 5: View the Results and verify the CONTENTS procedure 
         report lists the names of the SAS data sets that 
         were created.
*************************************************************/
%let path=/home/u62043935/sas_sql_essential1;

/*++++++++++++++++++++++++++++++++++++++++++++++++++++++++++++
 WARNING: DO NOT ALTER CODE BELOW THIS LINE UNLESS DIRECTED 
          TO DO SO BY YOUR INSTURCTOR.
+++++++++++++++++++++++++++++++++++++++++++++++++++++++++++*/

/*************************************************************
  Alternate Data Location paths:
*************************************************************/

*%let path=s:/workshop/sq1m6;
*%let path=c:/workshop/sq1m6_review;
*%let path=c:/SAS_Education/sq1m6;
*%let path=c:/SAS_Education/lwsq1m6;

%include "&path/data/setup.sas" / encoding=wlatin1;
```

this will load sas7dbat files in the data folder

<img width="457" height="1134" alt="image" src="https://github.com/user-attachments/assets/e1576b22-c2e9-4fb6-97fa-d968ae7b74b3" />

Then create libname 

```
%let path=/home/u62043935/sas_sql_essential1;
 
libname sq "&path/data";
```

library SQ will be created in Libraries

<img width="612" height="1104" alt="image" src="https://github.com/user-attachments/assets/2b34f8f8-ff65-4c65-820c-cca354a6f54c" />






# 1.3 Introduction to the SQL Procedure

















