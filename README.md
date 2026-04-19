**🟢 ZippyRide – Console-Based Ride Booking System**

**📌 Overview**

ZippyRide is a C# console application that simulates a real-world ride booking platform (similar to Ola). It supports three user roles: Customer, Driver, and Admin, each with dedicated functionalities. I developed during my internship period.

The system demonstrates booking workflows, OTP-based ride validation, and role-based access control.

**⚙️ Features**
**👤 Customer**
1. Sign up and login
2. Book rides (source, destination, distance, date, time)
3. View fare and OTP generation
4. View active ride
5. Ride history (Upcoming, Ongoing, Completed)

**🚗 Driver**
1. Sign up with vehicle and license details
2. View ride requests (broadcast system)
3. Accept ride (First Come First Serve)
4. Start ride using OTP
5. End ride
6. View active ride and ride history

**🛠️ Admin**
1. Verify drivers before activation
2. View all customers and drivers
3. Set price per kilometer
4. Manage platform data

**🔄 Workflow Highlights**
- Ride requests are broadcasted to all drivers
- Only one driver can accept a ride (race condition simulation)
- OTP is required to start the ride
- Ride lifecycle: Requested → Accepted → Ongoing → Completed
  
**🧠 Concepts Used**
 - Object-Oriented Programming (OOP)
- Role-based system design
- Data validation
- State management
- Console-based UI design
- Basic concurrency simulation (First Come First Serve logic)

**🛠️ Tech Stack**
**Language**: C#
**Platform**: .NET Console Application
**Database**: SQL Server

**📷 Sample Flow**
1. Customer books a ride
2. Drivers receive broadcast request
3. One driver accepts
4. Customer receives driver details
5. OTP verification starts ride
6. Ride completes
