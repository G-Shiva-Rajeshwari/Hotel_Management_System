## Hotel Reservation System
Overview
This is a simple Java console application that connects to a PostgreSQL database to manage hotel room reservations. The system allows users to reserve rooms, view existing reservations, update or delete reservations, and retrieve room details by reservation ID.

# Features
Reserve a room by entering guest details and room number.

View all reservations with guest names, room numbers, contact info, and reservation dates.

Retrieve room number using reservation ID and guest name.

Update reservation details including guest name, room number, and contact number.

Delete reservations by reservation ID.

Exit the system with a countdown message.

# Technologies Used
Java 
JDBC for database connectivity
PostgreSQL database (assumed to be running locally)


# Database Setup
The application connects to a PostgreSQL database named HotelDB running locally. It uses a table named reservations with columns:

reservation_id (primary key, auto-increment)
guestname (text)
roomnumber (integer)
contactnumber (text)

# Make sure your PostgreSQL server is running and accessible with the following credentials:

URL: jdbc:postgresql://localhost:5432/DBName (database name as u created)

Username: postgres (for postgre)

Password: 


# How to Run
Ensure PostgreSQL database is up and the reservations table exists.

Compile the Java code:
Run the program:

Follow the on-screen menu to interact with the system.

Notes
The system assumes room numbers between 1 and 150.

Basic input validation is included.

Uses JDBC Statement for SQL queries; be cautious of SQL injection in a production environment.

Proper exception handling is in place to catch database errors.

