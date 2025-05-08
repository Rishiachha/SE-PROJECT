# SE-PROJECT
NOTE:Kindly see this readme file in code formate not in preview because you will understand how your foulder structure should be which will make clear understanding

structure of the project
├── controller
│   └── registrationController.js    
├── database
│   └── database.js                 
├── model
│   ├── courseRegistration.js       
│   └── user.js                    
├── public
│   ├── login.html                 
│   ├── signup.html                 
│   ├── dashboard.html             
│   ├── student.html                
│   ├── courseopenelective.html     
│   ├── projects.html              
│   ├── confirmation.html           
│   └── admin.html                  
├── route
│   └── registrationRoutes.js                            
├── package.json                    
├── package-lock.json               
├── server.js  

synopsis : A web application for students to register for courses and projects, with admin functionality to manage registrations. Built with Node.js, Express, MongoDB, and a frontend using HTML, CSS, and JavaScript, this system allows users to sign up, log in, select course/project preferences, and view confirmations, while admins can oversee all registrations.

Features
User Authentication: Sign up and log in with role-based access (student/admin).
Course Registration: Students can select up to 5 open elective courses.
Project Registration: Students can select up to 5 project preferences.
Registration Management: Students can view, edit, or delete their registrations; admins can view/delete all registrations.
Responsive Frontend: Dashboards, confirmation pages, and forms for a seamless user experience.
Secure Backend: Password hashing with bcrypt and environment-based MongoDB credentials.

installing Prerequisites
To run this project, ensure you have the following software installed:
Node.js (v16.20.1 or higher): JavaScript runtime for the backend.
MongoDB: Local MongoDB server or a cloud service like MongoDB Atlas.
Git: For cloning the repository.
Web Browser: Chrome, Firefox, or any modern browser for accessing the frontend.
Code Editor: VS Code or any editor for modifying code

Notes
Security: Passwords are hashed using bcrypt. Ensure your MongoDB connection string is kept secure in the .env file.
Frontend: The frontend assumes the backend API is running at http://localhost:3000. Update API URLs in HTML files if deploying to a different host.
Cloudflare Script: HTML files include a Cloudflare bot protection script, which may be unnecessary for local development. Remove it if it causes issues (search for <script>(function(){function c(){ in HTML files).
Database: If using MongoDB Atlas, ensure your IP is whitelisted in the Atlas dashboard.
Testing: Test the application locally before deploying to ensure all features work as expected

Technologies
Backend: Node.js, Express, MongoDB, Mongoose
Frontend: HTML, CSS, JavaScript

Dependencies:
express: Web framework
mongoose: MongoDB ORM
cors: Cross-origin resource sharing
dotenv: Environment variable management
bcrypt: Password hashing

Troubleshooting
MongoDB Connection Error: Verify your MONGO_URI in .env and ensure MongoDB is running or Atlas is accessible.
CORS Issues: Ensure the backend (server.js) includes cors middleware.
API Errors: Check browser console for errors and ensure the server is running at http://localhost:3000.
Port Conflict: If port 3000 is in use, update the port variable in server.js.

