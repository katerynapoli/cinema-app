# Cinema App 📽️

### Project description:
```
A simple web-application that supports registration, authentication and other CRUD operations.
```

## 🎯 Features:

- registration and authentication as an admin or a user

As ```admin``` you can:
- add / get all cinema halls
- add / get all movies
- add / update / delete / find an available movie sessions
- find a user by email

As ```user``` you can:
- get all cinema halls
- get all movies
- find an available movie sessions
- complete an order / get an order history
- add a movie session to your shopping cart / get your shopping cart

## 💿 Required Software:
1. [JDK 19](https://jdk.java.net/19/)
2. [Apache Maven 3.8](https://maven.apache.org/download.cgi)
3. [MySQL 8.0.32](https://dev.mysql.com/downloads/mysql/)
4. [Tomcat 9.0](https://tomcat.apache.org/download-90.cgi)
5. [IntelliJ Idea](https://www.jetbrains.com/idea/download/#section=mac) (Ultimate Edition)
6. [MySQL Workbench](https://www.mysql.com/downloads/) (Optional)

## 🤖 Technologies
1. Servlet API
2. JPA
3. JDBC API
4. Hibernate
5. Spring Framework
6. Apache Tomcat
7. MySQL

## ⚙️ Getting Started:
1. Copy HTTPS / SSH of the project via clicking on the ```<>Code``` button
2. Open IntelliJ Idea and choose to create a new ```Project from Version Control```
3. Paste your HTTPS / SSH
4.
- If you are using MySQL Workbench:
  - Set up a new connection (set your username and password, you will need them later)
  - ```Test Connection```
  - Open your freshly made connection and create a new schema, for example ```cinema_app```
  - Hibernate will automatically populate it with all necessary tables after running the App


- If you are using ```Database``` tab in IntelliJ Idea:
  - Press ```Plus ➕``` and choose MySQL as ```Data Source```
  - Set your username and password (you will need them later)
  - ```Test Connection```
  - Create a new schema using MySQL ```console``` (it will open automatically)
  - Query like this will do the job: CREATE SCHEMA \`cinema_app` DEFAULT CHARACTER SET utf8 ;
  - Hibernate will automatically populate it with all necessary tables after running the App

5. Open ```cinema-app/src/main/resources/db.properties```
6. Insert your driver instead of *YOUR_DRIVER*, for example: ```com.mysql.cj.jdbc.Driver```
7. Insert a URL of your DB instead of *YOUR_DATABASE_URL*, for example: ```dbc:mysql://localhost:3306/cinema_app?serverTimezone=UTC```
8. Insert your username and password instead of *YOUR_USERNAME* and *YOUR_PASSWORD* respectfully (set to your DB earlier)
9. Click ```Current File ▾``` tab to Select Run/Debug Configuration, then ```Edit Configurations```
10. Click ```Plus ➕```, ```Tomcat Server```, ```Local```
11. In the pop-up window click ```Fix``` and choose ```cinema-app:war exploded```
12. Set ```Application context``` to ```/```
13. Run ```mvn clean package``` in the terminal
14. After pressing ```Run Tomcat ▶️``` button a new window with the application will open in your browser
15. You are successfully set up for using the Cinema App 🎉
