🟢 ZippyRide – Console-Based Ride Booking System
📌 Overview

ZippyRide is a C# console application that simulates a real-world ride booking platform (similar to Ola). It supports three user roles: Customer, Driver, and Admin, each with dedicated functionalities.

The system demonstrates booking workflows, OTP-based ride validation, and role-based access control.

⚙️ Features
👤 Customer
Sign up and login
Book rides (source, destination, distance, date, time)
View fare and OTP generation
View active ride
Ride history (Upcoming, Ongoing, Completed)
Profile management
🚗 Driver
Sign up with vehicle and license details
View ride requests (broadcast system)
Accept ride (First Come First Serve)
Start ride using OTP
End ride
View active ride and ride history
🛠️ Admin
Verify drivers before activation
View all customers and drivers
Set price per kilometer
Manage platform data
🔄 Workflow Highlights
Ride requests are broadcasted to all drivers
Only one driver can accept a ride (race condition simulation)
OTP is required to start the ride
Ride lifecycle: Requested → Accepted → Ongoing → Completed
🧠 Concepts Used
Object-Oriented Programming (OOP)
Role-based system design
Data validation
State management
Console-based UI design
Basic concurrency simulation (First Come First Serve logic)
🛠️ Tech Stack
Language: C#
Platform: .NET Console Application
Database: (mention yours — SQL / in-memory / file-based)
📷 Sample Flow
Customer books a ride
Drivers receive broadcast request
One driver accepts
Customer receives driver details
OTP verification starts ride
Ride completes
