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

6.Features and Functionality:
Authentication and User Roles:

Students: Can register, wait for admin approval, login, book appointments, and manage profiles.
Teachers: Admin adds teachers. Teachers manage availability, handle appointment requests, and communicate with students.
Admin: Manages teacher registrations and student approvals.
Responsive Design: The project is fully responsive and works on all devices (smartphones, tablets, laptops, and desktops).

Messaging: Students and teachers can send messages related to appointments.

Scheduling: Teachers can set available time slots for students to book appointments.
