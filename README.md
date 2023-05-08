![markdown logo](https://eww-wp-new.s3.ap-south-1.amazonaws.com/wp-content/uploads/2021/02/19100650/online-movie-ticket-booking-app-development.png)
# 🎞 CINEMA APP

Cinema app is a web application that allows users to view the schedule of movie sessions and purchase tickets for them. 
The application has a user registration system and a secure section with access rights to various resources based on user roles. 
Additionally, users can obtain information about movies available at the cinema, including their descriptions. 
The app is built on the concept of REST and uses the Spring and Hibernate frameworks to ensure a smooth and efficient user experience. 
Whether you're a regular user or an admin, our app provides role-based authorization to ensure that everyone has access 
to the appropriate resources.

## ⚙️ Install

- Clone this remote repository to your local repository :
  <br>`git clone https://github.com/pechivo/cinema-app.git`
- Update fields JDBC_DRIVER, URL, USERNAME, PASSWORD with your database connection information in
  <br>`in db.properties (resource directory)` with the appropriate values for your database setup
- Build the project using Maven : `mvn clean install`
- Configure run with Tomcat

Now you can login as User or as Admin by such login information:
- for User - <br>`login: admin@gmail.com, password: Admin1234`
- for Admin - <br>`login: user@gmail.com, password: User1234`

## 🎯 Features

As a registered user with the USER role, you will have access to the following features:

- Browse and search for movies and cinema halls. 
- Find available movie sessions based on your preferred date and time. 
- Create a shopping cart to add selected movie tickets. 
- View and manage the contents of your shopping cart. 
- Place an order for the selected tickets. 
- Access your order history to review previous purchases.

As an ADMIN role user, you will have additional privileges, including:

- Create and manage movies and cinema halls in the system. 
- Create and manage available movie sessions for different movies and cinema halls. 
- Conveniently find a specific user by their email address for administrative purposes.

## 🛠 Structure:
Our cinema app has a structured architecture that is organized as follows:

<br>`Config`: stores the Spring configuration used by the application.
<br>`Controller`: contains the endpoints for the app's web interface.
<br>`DAO`: the Data Access Layer (Repository) responsible for performing CRUD (Create, Read, Update, Delete) operations 
in the database.
<br>`DTO`: a data transfer object that wraps model objects to standardize the requests and responses received and sent 
by controllers.
<br>`Lib`: contains email and password validators with corresponding annotations for convenience.
<br>`Model`: contains the models used by the application to represent entities in the database.
<br>`Service`: contains services that invoke the DAO and Authentication classes for database operations and user 
authentication, respectively.
<br>`Mapper`: converts model objects to DTO objects for smooth data transfer.
<br>`Util`: utility class used to determine DateTime pattern.

## 🛠 Used technologies:

- JDK 17 version
- Maven 3.10.1 version
- Spring 5.3.20 version
- Spring Security 5.6.10 version
- MySql 8.0.22 version
- Hibernate 5.6.14.Final 
- Hibernate Validator 6.1.6.Final
- Jackson core v.2.14.1 
- Javax annotation v.1.3.2
- Java Servlets 4.0.1 version
- Apache Tomcat 9.0.73 version

<br>

#### Have a nice cinema app experience 🎥 