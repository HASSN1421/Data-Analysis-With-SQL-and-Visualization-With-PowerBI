# Project Title



# Dashboard  For HR Department about employees details in organiza



## Problem Statement
 The Human Resources Department wants a report from you according to the following requirements  
- Total employees by department and section
- Know the details of employees’ ages by gender 
- Average sick leave by gender and age group 
- Details of employees by Shift by  gender and age
- A table containing employee details
- The age division is (30-40, 40-50, and 50-60)
 ### Steps followed
- Step 1 : Understanding and analyzing requirements
 - Step 2 : Review the data and identify the tables and columns I need in the report
   ![لقطة شاشة 2024-06-06 112054](https://github.com/HASSN1421/Data-Analysis-With-SQL-and-Visualization-With-PowerBI/assets/162873878/71002e5c-fbdf-4582-876e-837a26f22398)




   
 - Step 3 : Understand relationships and write a query to collect data
  - Step 4 : Add the operations I need in the query to build the report 
       
   
         -Includes date formatting:
         FORMAT(D.ModifiedDate,'dd/mm/yyyy') as D_ModifiedDate
         -Merge columns: 
         CONCAT(P.FirstName,'  ',P.LastName) as full_name
         -Age calculation:

         DATEDIFF(YEAR,ED.BirthDate,GETDATE()) as age
         -Determine the age group:

         CASE 
              WHEN DATEDIFF(YEAR,ED.BirthDate,GETDATE()) BETWEEN 30 AND 40 THEN '30 to 40'

                   WHEN DATEDIFF(YEAR,ED.BirthDate,GETDATE()) BETWEEN 41 AND 50 THEN '41 to 50'

                   	 WHEN DATEDIFF(YEAR,ED.BirthDate,GETDATE()) BETWEEN 51 AND 60 THEN '51 to 60'
                          ELSE 'Above 60'

                          END as age_categor







 - Step 5 : Create a view for the query
     
     ![لقطة شاشة 2024-06-06 120028](https://github.com/HASSN1421/Data-Analysis-With-SQL-and-Visualization-With-PowerBI/assets/162873878/cac3c79b-2eb0-4c58-9815-717e8845eb4a)
 - Step 6 : get data from SQL server  into  PowerBI



![لقطة شاشة 2024-06-06 120349](https://github.com/HASSN1421/Data-Analysis-With-SQL-and-Visualization-With-PowerBI/assets/162873878/b7c0eba2-735a-453a-be24-ed130cbe942d)

 - Step 7 : Create chart for all requirements includes


       
        .chart for Total employees by department and Administration
      ![لقطة شاشة 2024-06-06 124155](https://github.com/HASSN1421/Data-Analysis-With-SQL-and-Visualization-With-PowerBI/assets/162873878/2f116158-11ac-435d-a07a-c5fb030e9e86)


       .Know the details of employees’ ages by gender 
     ![لقطة شاشة 2024-06-06 124531](https://github.com/HASSN1421/Data-Analysis-With-SQL-and-Visualization-With-PowerBI/assets/162873878/875808d6-d2c1-4da3-b3d9-cbaedda7299e)

       .Average sick leave by gender and age group 
    ![لقطة شاشة 2024-06-06 124836](https://github.com/HASSN1421/Data-Analysis-With-SQL-and-Visualization-With-PowerBI/assets/162873878/727fd8db-5561-4d58-b832-7252d1376176)


    ![لقطة شاشة 2024-06-06 124934](https://github.com/HASSN1421/Data-Analysis-With-SQL-and-Visualization-With-PowerBI/assets/162873878/d65f7062-ac2d-44e2-9696-56047e0f4060)


       .Details of employees by Shift by  gender and age
    ![لقطة شاشة 2024-06-06 125121](https://github.com/HASSN1421/Data-Analysis-With-SQL-and-Visualization-With-PowerBI/assets/162873878/7d00e212-db52-4a12-a635-b641e9baed96)


    ![لقطة شاشة 2024-06-06 125207](https://github.com/HASSN1421/Data-Analysis-With-SQL-and-Visualization-With-PowerBI/assets/162873878/49f2d51c-e6a8-44ac-af09-f1e61ed0d2b0)


       .A table containing employee details
   ![لقطة شاشة 2024-06-06 125413](https://github.com/HASSN1421/Data-Analysis-With-SQL-and-Visualization-With-PowerBI/assets/162873878/e5062945-6732-4929-a700-c0990479c862)


 

 ### Final format of the report
 ![لقطة شاشة 2024-06-06 125601](https://github.com/HASSN1421/Data-Analysis-With-SQL-and-Visualization-With-PowerBI/assets/162873878/d5ce755c-e19f-4cea-906f-b837d56a247d)







