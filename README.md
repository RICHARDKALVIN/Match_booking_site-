# Matchbookingsite  

```markdown
# RIVIN Cricket Club Web Application

## Overview

The **RIVIN Cricket Club** web application is designed to manage cricket match details, player registrations, and audience ticket bookings. The platform allows admins to add match information, players to register, and audiences to view match details and book tickets.

## Features

**Admin Portal**  
Admins can add match details, including teams, venue, date, and time.  

**Player Portal**  
Players can register for matches.  

**Audience Portal**  
Audiences can view match details and book tickets.  

## Tech Stack

**Frontend:** HTML, CSS  
**Backend:** Java, Servlets (Using Apache Tomcat 10.1.28)  
**Database:** MySQL (Managed via MySQL Workbench)  
**Server:** Apache Tomcat 10.1.28  

## Database Setup

1. Install **MySQL Workbench** and **MySQL Server**.  
2. Create a new database:  
   
   CREATE DATABASE cricket_club;
   
3. Create required tables:  
  
  CREATE TABLE MatchInfo (
    match_id INT AUTO_INCREMENT PRIMARY KEY,
    match_name VARCHAR(50),
    match_date DATE,
    place VARCHAR(50)
);




  CREATE TABLE Register (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(100),
    dob DATE,
    city VARCHAR(50),
    gender ENUM('Male', 'Female', 'Other'),
    age INT
);




CREATE TABLE TicketBooking (
    booking_id INT AUTO_INCREMENT PRIMARY KEY,
    match_name VARCHAR(50),
    user_name VARCHAR(100),
    ticket_count INT
);

   
4. Configure MySQL database connection in the Java backend.  

## How to Run

1. Clone the repository:  
   ```sh
   git clone https://github.com/your-username/ALK-Cricket-Club.git
   ```
2. Open the project in **Eclipse**.  
3. Configure **Apache Tomcat 10.1.28**.  
4. Run the application.  
5. Access the web app at: `http://localhost:8080/myfirstwebapp/index.html`  

## Screenshots
### Home Page:
![Screenshot (182)](https://github.com/user-attachments/assets/d85f4016-07e4-40c0-9f15-0fffe1d9c0ff)

### Add match Page:

![Screenshot (183)](https://github.com/user-attachments/assets/562d281b-eb6f-4a5b-9ba3-1a3e14b6c2d6)


![Screenshot (189)](https://github.com/user-attachments/assets/f9709807-acc6-4fd1-9eac-cfef44d920aa)

### Match View Page:

![Screenshot (186)](https://github.com/user-attachments/assets/ed12ba56-ec51-4132-8063-76567aeee23d)

### Register Page:

![Screenshot (184)](https://github.com/user-attachments/assets/9990cb5b-eaf7-43dc-aa4e-f91047e4a24f)

### BOOKING Page:
![Screenshot (187)](https://github.com/user-attachments/assets/32329456-53a2-42e0-a793-a955afe74622)

 


### Suceess Page:
 
![Screenshot (185)](https://github.com/user-attachments/assets/6354b2ec-b013-4f7a-b0d1-91e1f46a81ad)

### ERROR Page:
![Screenshot (192)](https://github.com/user-attachments/assets/3219e17b-630d-4cbd-b30b-898fe2c2cdbf)

![Screenshot (193)](https://github.com/user-attachments/assets/63327dd3-2588-4aa7-829d-eabb7a2446f8)



## Contributing

Feel free to contribute by submitting issues or pull requests.  

## License

This project is licensed under the MIT License.  
```
 
