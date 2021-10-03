# To create table
Create Table(
 Name_VARCHAR(255),
 Customer_ID VARCHAR(18),
 Open_Date Date(8),
 Last_Consulted Date(8),
 Vaccinated_ID Char(5),
 Dr_Name Char(255),
 State Char(5),
 Country Char(5),
 DOB Date(8),
 Is_Active Char(1),
 );
 #Insert into table
 INSERT INTO Table(Name,Customer_ID,Open_Date,Last_Consulted,Vaccinated_ID,Dr_Name,State,Country,DOB,Is_Active)
 VALUES('Alex','123457','20101012','20121013','MVD','Paul','SA','USA',06031987,'A');
 INSERT INTO Table(Name,Customer_ID,Open_Date,Last_Consulted,Vaccinated_ID,Dr_Name,State,Country,DOB,Is_Active)
VALUES('John','123458','20101012','20121013','MVD','Paul','TN','IND','06031987','A');
 INSERT INTO Table(Name,Customer_ID,Open_Date,Last_Consulted,Vaccinated_ID,Dr_Name,State,Country,DOB,Is_Active)
VALUES('Mathew','123459','20121013','MVD','Paul','WAS','PHIL','06031987','A');
 INSERT INTO Table(Name,Customer_ID,Open_Date,Last_Consulted,Vaccinated_ID,Dr_Name,State,Country,DOB,Is_Active)
VALUES('Matt','12345','2010101','20121013','MVD','Paul','BOS','NYC','06031987','A');
 INSERT INTO Table(Name,Customer_ID,Open_Date,Last_Consulted,Vaccinated_ID,Dr_Name,State,Country,DOB,Is_Active)
VALUES('Jacob','1256','20101012','20121013','MVD','Paul','VIC','AU','06031987','A');
#SPLIT countrywise
SELECT Count(Customer_ID),Country
 from Table
 Group By Country
 
 file=open(r"SQL","r")
