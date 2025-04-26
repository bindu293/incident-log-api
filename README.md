
📋 Incident Log API

A simple, clean **Spring Boot + Java + MySQL** REST API to manage incident reports.
✨ Features
- Create, view, delete incidents
- Connects to a real MySQL database
- Pre-loaded sample incidents
- Exception handling (404 if incident not found)
- Professional project structure (Model-Service-Repository-Controller)

 🛠️ Tech Stack
- Java 17
- Spring Boot 3.x
- Spring Data JPA
- MySQL Database
- Maven

📂 Project Structure

src/
    main/
        java/
            org.example
              controller/
               model/
               repository/
               service/
               exception/
       resources/
          application.properties

          
 🚀 How to Run

1. Make sure you have:
   - Java 17+
   - Maven
   - MySQL Server running

2. Clone this repository:
   
   in bash
   
   git clone https://github.com/your-username/incidentlogapi.git
   
   cd incidentlogapi
   

4. Create a MySQL database:
   
   CREATE DATABASE incidentdb;

5. Configure `src/main/resources/application.properties`:
 
MySQL Database Configuration

spring.datasource.url=jdbc:mysql://localhost:3306/your_db

spring.datasource.username=your_mysql_username

spring.datasource.password=your_mysql_password

spring.jpa.hibernate.ddl-auto=update

spring.jpa.show-sql=true

spring.jpa.properties.hibernate.dialect=org.hibernate.dialect.MySQL8Dialect

✅ Replace `your_mysql_username` and `your_mysql_password` accordingly.

5. Build the project:

   
   mvn clean install
   

7. Run the project:

   
   mvn spring-boot:run
   

9. App will start at:
    
   http://localhost:5050

 📚 API Endpoints
 
 GET  /api/incidents  Get all incidents 
 
 GET /api/incidents/{id}  Get incident by id 
 
 POST  /api/incidents  Create new incident 
 
 DELETE /api/incidents/{id}  Delete incident by id 
 
Postman-

📬 Example Requests

 ➡️ Get all incidents
 
 GET http://localhost:5050/api/incidents
 
➡️ Get incident by ID

 GET http://localhost:5050/api/incidents/1
 
 ➡️ Create new incident
 
 POST http://localhost:5050/api/incidents 
 
-Header "Content-Type: application/json" 

-description 
{
  "title": "Server Crash",
  
  "description": "The server went down during heavy traffic.",
  
  "severity": "High"
}

➡️ Delete incident

 DELETE http://localhost:5050/api/incidents/1
 
⚡ Author
Made with ❤️ by **Bindu sree**

 🌟 Ready to 🚀
This project shows you understand full backend development —  
building services, databases, APIs, exception handling 

