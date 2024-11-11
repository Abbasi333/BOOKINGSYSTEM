-------------------------------------------------------------------
SET PROJECT LOCALLY:
1. Clone the Repository:
   Clone the repository to your local machine using the following command:
   git clone <REPO LINK>
2. Install Dependencies:
   Navigate into the project folder and install the required dependencies.
   cd student-teacher-booking-appointment
   npm install
3. Set Up Firebase:
   Create a Firebase project in the Firebase Console.
   In the Firebase console, enable Firestore Database and Authentication.
   Get your Firebase configuration object from your Firebase project settings and add it to your project under the src/firebase/config.js file.
4. Start the Application Locally:
   To run the project locally, use the following command:
   npm start
   This will start the application and open it in your default web browser at http://localhost:3000.
5. Access the Application:
   Login as a Student: After registration (admin approval required), you can login and book appointments.
   Login as a Teacher: Admin will add teachers who can then manage availability and appointments.
   Login as Admin: The admin can manage user registrations and teacher approvals.
----------------------------------------------------------------------
FOLDER STRUCTURE:
public/
├── index.html # HTML template for the app
├── style.css # Global styling file
└── app.js # Entry point for React application

src/
├── pages/
│ ├── Navigation/ # Navbar components
│ ├── Authorization/ # Login and registration components
│ ├── Admin/ # Admin dashboard components
│ ├── Teacher/ # Teacher dashboard components
│ └── Student/ # Student dashboard components
└── index.js # Main entry point for React app
-------------------------------------------------------------------------
6.Features and Functionality:
Authentication and User Roles:

Students: Can register, wait for admin approval, login, book appointments, and manage profiles.
Teachers: Admin adds teachers. Teachers manage availability, handle appointment requests, and communicate with students.
------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
          BOOKING SYSTEM:
TOOLS:
•	React.js
•	Node.js
•	Firebase
Description
•	Appointment booking systems, whether online or traditional, are crucial for efficient scheduling in various industries.
•	Web-based solutions enhance accessibility and reduce wait times.
•	This project introduces a web platform enabling students and teachers to schedule appointments seamlessly.
•	It ensures easy access via web or mobile, allowing users to manage appointments and communicate effectively, thereby improving scheduling efficiency and user convenience.
Project Summarization:
The Student Teacher Booking Appointment project offers a streamlined web-based solution for students and teachers to manage appointment scheduling effortlessly.
Built on React with Firebase integration, it provides secure login authentication, role-based dashboards (admin, teacher, student), and features like scheduling, messaging, and profile management.
Ideal for educational institutions, it enhances communication and efficiency in scheduling appointments.
SYSTEM EXPLANATION:
Frontend (React Application):
The frontend is built using React, which interacts with the users (students, teachers, and admins) through a web interface.
React Router is used for navigation between different views (e.g., login, registration, dashboards).
Student Portal:
Students can register and login after admin approval. They can book appointments with teachers, view available slots, and communicate with teachers through messages.
Teacher Portal:
Teachers can log in and manage their availability schedules, handle appointment requests, and communicate with students via messages. They can also update their profile.
Admin Portal:
Admins can manage teacher registrations, approve student accounts, and oversee the general functioning of the system. Admin has restricted access but can manage teacher availability and student registrations.
Firebase Firestore (Database):
Firebase Firestore is used to store data related to users (students, teachers, admins), appointments, messages, and availability. Firestore is a NoSQL database that allows real-time synchronization of data across the platform.
Authentication & Role-based Access:
Firebase Authentication is used for secure login (via email/password). Different roles (student, teacher, admin) have access to different parts of the system based on their authentication and authorization.

Admin: Manages teacher registrations and student approvals.
Responsive Design: The project is fully responsive and works on all devices (smartphones, tablets, laptops, and desktops).

Messaging: Students and teachers can send messages related to appointments.

Scheduling: Teachers can set available time slots for students to book appointments.
