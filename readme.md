✨ Smart Contact Manager

Tech Stack:

Frontend: HTML5, CSS3, JavaScript
Backend: Spring Boot, Hibernate
Database: MySQL
Build Tool: Maven
Authentication: Spring Security, Google OAuth, GitHub OAuth


⚙️ Features
🔒 Secure Authentication (Email, Google, GitHub)
📇 Contact Management (CRUD operations)
🌐 RESTful APIs
💻 Responsive UI

🚀 Setup
Clone Repo:
git clone https://github.com/omborhade/SCM-2.0
cd SCM-2.0

Configure MySQL:
CREATE DATABASE contact_manager_db;

Update application.properties :
spring.datasource.url=jdbc:mysql://localhost:3306/contact_manager_db
spring.datasource.username=your_username
spring.datasource.password=your_password

Run Project:
mvn clean install
mvn spring-boot:run

Access: Open http://localhost:8080 in your browser.

📌 API Endpoints
Auth:

POST /signup
POST /login
Contacts:

GET /api/contacts
POST /api/contacts
PUT /api/contacts/{id}
DELETE /api/contacts/{id}
GET /api/contacts/search?query=xyz

🤝 Contributing
Fork, issue, pull request
