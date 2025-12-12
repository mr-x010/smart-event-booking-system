Project Overview
Smart Event Booking System is a MERN + MySQL application where users can browse upcoming events, view seat availability, and book tickets, while admins can manage events and track reservations.​

Tech Stack
Frontend: React, JavaScript, CSS (or Tailwind CSS if used).​

Backend: Node.js, Express.js, MySQL.​

Database: MySQL with event_booking_db containing events and bookings tables.​

How to Run Backend (server)
Install dependencies:

bash
cd server
npm install
Create a .env file inside the server folder with your MySQL configuration, for example:

DB_HOST=localhost

DB_USER=your_mysql_user

DB_PASSWORD=your_mysql_password

DB_NAME=event_booking_db

Start the backend server:

bash
npm start
or use the script defined in server/package.json (for example npm run dev).

How to Run Frontend (client)
Install dependencies:

bash
cd client
npm install
Start the React app:

bash
npm start
or

bash
npm run dev
Open the URL shown in the terminal (for example http://localhost:3000 or http://localhost:5173).

Database Setup (MySQL)
Open MySQL Workbench (or any MySQL client).​

Create the database if it does not exist:

sql
CREATE DATABASE event_booking_db;
Import the schema from the event_booking.sql file in the project root:

Go to Server → Data Import.

Choose Import from Self-Contained File and select event_booking.sql.

Select the target schema event_booking_db.

Click Start Import.​​

Main Features
List of events with title, description, location, date, price, total seats, and available seats.​

Event details page with booking form.​

Bookings store user details (name, email, mobile), quantity, total amount, and booking status (confirmed or cancelled).​

Admin APIs for creating, updating, and deleting events.
