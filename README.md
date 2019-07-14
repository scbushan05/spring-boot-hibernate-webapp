# Spring boot, Hibernate and MySQL webapp

The  goal of the application is to create a web application with Spring boot, hibernate and MySQL. This application not used JPA or JPA specific methods instead we used Native Hibernate.

## Tools and Technologies used

* Java 1.8
* Spring boot 2.1.1
* Hibernate 5.3.7
* MySQL 8.0.13
* Eclipse Oxygen

## Steps to install

**1. Clone the application**

```bash
https://github.com/scbushan05/spring-boot-hibernate-webapp.git
```

**2. Create MySQL database**

```sql
CREATE DATABASE crudapi
```

**3. Create table or run the sql script file**

```sql
CREATE DATABASE crudapi;

USE crudapi;

CREATE TABLE tbl_employee
(
	id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
    name VARCHAR(255),
    gender VARCHAR(255),
    department VARCHAR(255),
    dob DATE
);
```

**4. Change MySQL username and password as per your installation**

+ open `src/main/resources/application.properties` file.

+ change `spring.datasource.username` and `spring.datasource.password` as per your installation

**5. Run the app**

You can run the spring boot app by typing the following command -

```bash
mvn spring-boot:run
```

You can also package the application in the form of a `jar` file and then run it like so -

```bash
mvn package
java -jar target/springbootcrudapi-0.0.1-SNAPSHOT.jar
```

The server will start on port 8080.

## Learn more

You can find the `video tutorial` for this application on my youtube channel -

<https://www.youtube.com/playlist?list=PLA7e3zmT6XQXIFcweUahWz2rQtmeI8dnl/>

You can find the tutorial for this application on my blog -

<https://bushansirgur.in/complete-crud-application-with-spring-boot-hibernate-and-mysql/>

You can subscribe to our Youtube channel -

<https://www.youtube.com/b2tech/>

You can join our free udemy courses also -

<https://udemy.com/user/bushansirgur/>
