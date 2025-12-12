-Project Overview
  .Smart Event Booking System built with React (client), Node.js/Express (server), and MySQL database event_booking_db.​

  .Users can view upcoming events, see seat availability, and book tickets; admins can create, update, and delete events.​

-Tech Stack
  .Frontend: React, JavaScript, CSS (Tailwind or normal CSS as used in this project).​

  .Backend: Node.js, Express.js, MySQL.​

  .Database: MySQL with tables events and bookings.​

-How to Run Backend (server)
  .Install dependencies:

-bash
 cd server
 npm install
 -Create a .env file inside the server folder with your MySQL config, for example:
  .DB_HOST=localhost

  .DB_USER=your_mysql_user

  .DB_PASSWORD=your_mysql_password

  .DB_NAME=event_booking_db

-Start backend server:
npm start
or use the script defined in server/package.json (for example npm run dev if configured).

-How to Run Frontend (client)
 .Install dependencies:

  .cd client
  .npm install
  
-Start React app:
  .npm start
 or


npm run dev
Then open the URL shown in the terminal (for example http://localhost:3000 or http://localhost:5173).

Database Setup (MySQL)
Open MySQL Workbench (or any MySQL client).​

Create database if not present:

sql
CREATE DATABASE event_booking_db;
Import the schema using the event_booking.sql file in the project root:

Go to Server → Data Import.

Choose Import from Self-Contained File and select event_booking.sql.

Select target schema event_booking_db.

Click Start Import.​​

Main Features
List of upcoming events with title, description, location, date, price, total seats, and available seats.​

Event detail page with full information and booking option.​

Booking API stores user details (name, email, mobile), quantity, total amount, and booking status (confirmed/cancelled).​

Admin can manage events (create, update, delete) through backend APIs.​

API Endpoints (Summary)
POST /events – Create event (admin).​

GET /events – Get all events with search and filters.​

GET /events/:id – Get single event details.​

PUT /events/:id – Update event (admin).​

DELETE /events/:id – Delete event (admin).​

POST /bookings – Create a new booking.​








