Smart Contact Manager
Key Skills: Spring Boot, Hibernate, MySQL, HTML5, CSS3, JavaScript

This project is a Smart Contact Manager web-based application developed using HTML5, CSS3, JavaScript for the frontend, and Spring Boot with Hibernate for the backend. The application enables users to securely manage their contacts with features like viewing, updating, deleting, and searching contacts. User authentication is implemented with email, Google, and GitHub integration.

Features
Secure User Authentication:
Users can sign up and log in via email, Google, or GitHub.
Email verification link during signup to confirm valid users.
Contact Management:
Create, view, update, delete, and search contacts.
User-specific contact storage (each user can manage their own set of contacts).
RESTful APIs:
Designed and implemented REST APIs to handle contact operations.
Responsive Frontend:
Built using HTML5, CSS3, and JavaScript for a smooth and user-friendly interface.
Database Management:
Contact data is stored securely in a MySQL database.
Hibernate is used as the ORM tool for efficient database interactions.
Tech Stack
Frontend: HTML5, CSS3, JavaScript
Backend: Spring Boot, Hibernate
Database: MySQL
Build Tool: Maven
Authentication: Spring Security, Google OAuth, GitHub OAuth
IDE: Eclipse, IntelliJ IDEA
Testing Tool: Postman (for API testing)

Setup and Installation

Prerequisites
Ensure the following are installed on your system:
Java 8 or higher
Maven
MySQL
Google and GitHub developer accounts for OAuth authentication setup

Steps to Run the Project

Clone the repository:
git clone https://github.com/omborhade/SCM-2.0
cd SmartContactManager
Configure the MySQL Database:

Create a MySQL database:
CREATE DATABASE contact_manager_db;
Update the database connection details in the application.properties file:
spring.datasource.url=jdbc:mysql://localhost:3306/contact_manager_db
spring.datasource.username=your_username
spring.datasource.password=your_password
 
 
Configure Google and GitHub OAuth:
Update application.properties with your Google and GitHub OAuth credentials:
spring.security.oauth2.client.registration.google.client-id=your_google_client_id
spring.security.oauth2.client.registration.google.client-secret=your_google_client_secret

spring.security.oauth2.client.registration.github.client-id=your_github_client_id
spring.security.oauth2.client.registration.github.client-secret=your_github_client_secret


Build and Run the Project:
mvn clean install
mvn spring-boot:run

Access the Application:
Open your browser and navigate to http://localhost:8080.

API Endpoints
Authentication APIs:
/signup : Sign up with email and password.
/login : Log in with email, Google, or GitHub.
Contact Management APIs:
GET /api/contacts : Retrieve all contacts for a user.
POST /api/contacts : Add a new contact.
PUT /api/contacts/{id} : Update an existing contact.
DELETE /api/contacts/{id} : Delete a contact.
GET /api/contacts/search?query=xyz : Search for contacts by name or other details.
Usage
User Signup and Login: Users can sign up using email or log in via Google and GitHub. Email verification is required for email-based signup.
Manage Contacts: After logging in, users can manage their contacts, including adding, editing, deleting, and searching for contacts.
API Testing: Use Postman to test the various API endpoints for contact management.
Future Enhancements
Contact Grouping: Add support for grouping contacts into categories (e.g., family, work).
Advanced Search: Implement advanced search filters (e.g., by date added or location).
Notifications: Notify users about upcoming contact-related events (e.g., birthdays, anniversaries).
Mobile App: Integrate a mobile app for easier access on-the-go.
Contributing
We welcome contributions from the community! Please feel free to fork the repository, submit issues, or create pull requests.

License
This project is licensed under the MIT License. See the LICENSE file for details.

