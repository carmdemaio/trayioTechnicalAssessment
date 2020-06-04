# trayioTechnicalAssessment

This is a Json Export of my Tray.io workflow I built as part of an interview for an SA role at Tray.io in March of 2020. If you import this Json, the following readme file will also appear at the top of the workflow:

```
Carm DeMaio 
5/26-20 - 5/28/20
SA Technical Assessment for Tray.io
In the spirit of iPaaS I tried to do as much as possible without custom code. I followed the documentation when it came to checking if a value (in this usecase, the value 'title') may include multiple words or phrases; which reccomended using javascript:
https://tray.io/documentation/platform/useful-scripts/#checking-if-a-piece-of-text-contains-multiple-words-or-phrases-script-connector
However I modified the script to return a boolean instead. Line 4 of this script can be modified to  add more titles.6
```

Requirements:
```
The purpose of this use case is to grab a CSV file from an SFTP server, perform some data transformation, and then insert the rows into the MySQL database table.

Currently, the MySQL table is empty. We've created the relevant columns, a primary (id) and unique key (email).

The CSV file (/tray_candidate/dummy_customer_set_v1.1) has name stored as one field; please separate that in your data transformation into a First and Last name column in MySQL. There are also two date fields. Currently, they're stored in an easy to consume way in CSV format, but will not be easy to deal with in SQL. Please change the format to YYYY-MM-DD.

A new column should be created as a boolean to keep track of an executive. If you detect "Chief" or "Senior" or "President" in their title, the boolean should be set to True.

Lastly, an additional column should be created as a boolean to keep track of students. If you detect a ".edu" email address, please set the boolean to True.

It's expected that you do error checking when attempting to access the SFTP server, as well as checking to see if the MySQL server connection is alive. If you encounter an error, email yourself that the system is down, and terminate the workflow.
```

      
