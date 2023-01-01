<img src = "https://th.bing.com/th/id/R.93e45a85d55d229c24d7010cbb96b9dd?rik=b3MJaJPx9wj8ew&riu=http%3a%2f%2fwww.freeworldgroup.com%2fpaidimages3%2flarge3%2fmystery3.jpg&ehk=finGjnnfmogMc2DNoBxEa%2bXbVNgUZdNSUcunPnBKmPM%3d&risl=&pid=ImgRaw&r=0&sres=1&sresct=1" width = "1500">
<h1 align = 'center', style = 'font-size:48px'><strong>A Mystery in Fiftyville</strong></h1>

## Overview
The CS50 Duck has been stolen! The town of Fiftyville has called upon you to solve the mystery of the stolen duck. Authorities believe that the thief stole the duck and then, shortly afterwards, took a flight out of town with the help of an accomplice. Your goal is to identify:

- Who the thief is,
- What city the thief escaped to, and
- Who the thief’s accomplice is who helped them escape

All you know is that the theft took place on July 28, 2021 and that it took place on Humphrey Street.

How will you go about solving this mystery? The Fiftyville authorities have taken some of the town’s records from around the time of the theft and prepared a SQLite database for you, fiftyville.db, which contains tables of data from around the town. You can query that table using SQL SELECT queries to access the data of interest to you. Using just the information in the database, your task is to solve the mystery.

## Queries
1. Query crime_scene_reports to confirm that the information supplied is correct for the data. The insight here is that the crime took place at 10:15 am and everyone mentioned the bakery<br><br>
2. Find out from the interviews table where the transcript contains ‘bakery’. A summary of the information here is listed below:
   - One of the thieves withdrew money from the ATM on Leggett Street earlier that morning
   - They left the bakery at about 10:25 am (10 minutes later after the incident)
   - They plan to leave town with the earliest flight the following morning (from conversation < 60mins at about 10:25 am)<br><br>
3. Then, these were used to form the CTE queries as follows. The  queries answer the following:
   - The person that used the atm
   - Those that made the calls
   - Car owners that fit the description
   - Passengers who board flights
   - Airports involve <br><br>
4. Print the suspect table from the subqueries<br><br>
5. Finally, format the output and print the result

   
## Acknowledgment
- [Harvard University](https://cs50.harvard.edu/x/2022/psets/7/fiftyville/#a-mystery-in-fiftyville)