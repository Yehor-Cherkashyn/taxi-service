# Taxi Service

The Taxi Service is a project that simulates a taxi service. 
Users can add and delete car models, cars, and drivers. 
They can also assign drivers to specific cars, 
view all cars belonging to the current driver, and authenticate themselves.

## Features

<ul>
<li>Authentication</li>
<li>Create and delete car manufacturer</li>
<li>Create and delete cars</li>
<li>Create and delete drivers</li>
<li>Add drivers to specific cars</li>
<li>View all cars belonging to the current driver</li>
<li>View all cars, drivers, manufacturers</li>
</ul>

## Structure

<ul>
<li>controller: Servlets that handle HTTP requests and responses</li>
<li>dao: Data Access Object interfaces and their implementations</li>
<li>exception: Custom exceptions used in the project</li> 
<li>filter: Servlet Filters used to intercept requests and responses</li>
<li>model: Plain Old Java Objects (POJOs) that represent data</li>
<li>service: Service interfaces and their implementations that perform business logic</li>
<li>util: Utility class used in a project to create a database connection</li>
<li>resources: Non-Java files such as database scripts and configuration files</li> 
<li>webapp: Contains web resources such as CSS, and JSP files</li>
<li>WEB-INF: Contains configuration files for the web application</li>
<li>views: Contains JSP files used as views in the application
for cars, drivers, manufacturers, authentication
and include css files (that contains CSS files used in the application)</li>
</ul>

## Used technologies:

<ul>
<li>Java 
<li>Java Servlets 
<li>SQL 
<li>Maven
</ul>

## Getting Started

<ul>
<li>Clone the project repository to your local machine</li>
<li>Run the SQL script located in src/main/resources/init_db.sql to initialize the database</li>
<li>Replace the values of the URL, USERNAME, PASSWORD and JDBC_DRIVER properties 
with the appropriate values for your database setup</li>
<li>Build the project using Maven: mvn clean install</li>
<li>Deploy the generated WAR file to servlet container such as Tomcat</li>
</ul>

## Authors

Yehor Cherkashyn
