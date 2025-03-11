# Hospital Appointment System - Project Specification &amp; Marking Guide
 ## Project Overview:
The Hospital Appointment System is a full-stack web-based application that allows patients to book appointments with doctors while hospital administrators manage doctors and schedules.
The back-end MUST be a C# .net api. The front end can be built using Blazor, React, Angular or VUE. 
The back-end database MUST be a SQL relational database.
The login / authentication mechanism MUST use Microsoft’s Identity Platform from .net 8 (or 9) OR a cloud based authentication using OAUTH / Microsoft Entrata or Microsoft B2C.
## Functional Requirements:
For more detailed functional requirements, you are expected to deliver on at least 80% of user stories which have been added to the appendix.
## 2.1 User Roles & Authentication
- Patients: Can register, log in, book, view, and cancel appointments.
- Doctors: Can log in, view their schedules, approve or reject appointments. Doctors can create prescriptions for the patients. 
- Admins: Manage doctors, patients, and appointments.
## 2.2 User Management
- Secure patient registration and profile management.
- Admin-controlled doctor registration and schedule setup.
- Role-based authentication using Microsoft Identity.
  ## 2.3 Appointment Booking & Management
- Patients can book, view, and cancel appointments.
- Doctors can approve, reject, and complete appointments.
- Admins can view and manage all appointments.
- System prevents double booking and scheduling conflicts.
  ## 2.4 Notifications & Reminders 
- Email confirmation upon booking/cancellation 
- Automated reminders before an appointment.
  ## 2.5 Search & Filtering
- Patients can search for doctors by specialization or name.
- Appointments can be filtered by date, doctor, or status.
## Database Design & Security:
The database should include tables for Users, Doctors, Appointments, and Notifications. Ensure proper relationships, foreign keys, and data integrity constraints.
Security measures should include role-based access control, parameterized queries to prevent SQL injection (Use EF Core) , and password hashing for authentication (already handled).
