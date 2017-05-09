# Project 10 - Fortress Globitek

Time spent: 5 hours spent in total

> Objective: Create an intentionally vulnerable version of the Globitek application with a secret that can be stolen.

### Requirements

- [X] All source code and assets necessary for running app
- [X] `/globitek.sql` containing all required SQL, including the `secrets` table
- [X] GIF Walkthrough of compromise
- [X] Brief writeup about the vulnerabilities introduced below

### Vulnerabilities

Describe the vuln(s) here.
This app has a Username Enumeration and some inplmentation bug. There is only one authorized user in the database, which is 'secret' with the password 'secret'. In the login page, the error message will be red if the attacker try to enter 'secret' in the username but with wrong password. The error message for other wrong username will also give out another way to hack retrive the secret message, which is by typing nothing in username and password. When the attacker successfully log in, the ssecret message will appear.
<img src='http://i.imgur.com/OEnSCBM.gif' title='Video Walkthrough' width='800 x 400' alt='Video Walkthrough' />
