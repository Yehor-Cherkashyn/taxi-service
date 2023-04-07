# ![Tux, the Linux mascot](/logo.webp) Taxi Service

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

## Getting Started

<ul>
<li>Clone the project repository to your local machine</li>
<li>Run the SQL script located in <code>src/main/resources/init_db.sql</code> to initialize the database</li>
<li>Replace the values of the <code>URL</code>, <code>USERNAME</code>, <code>PASSWORD</code> and <code>JDBC_DRIVER</code> properties 
with the appropriate values for your database setup</li>
<li>Build the project using Maven: <code>mvn clean install</code></li>
<li>Deploy the generated WAR file to servlet container such as Tomcat</li>
</ul>

## Structure

<ul>
<li>controller: Servlets that handle HTTP requests and responses</li>
    <ul>
        <li>LoginController - <code>POST /login</code> - authentication</li>
        <li>LogoutController - <code>GET /logout</code> - invalidate current session</li>
        <li>IndexController - <code>GET /</code> - show all corresponding pages</li>
        <li>AddCarController - <code>POST /cars/add</code> - adds a new car</li>
        <li>AddDriverToCarController - <code>POST /cars/drivers/add</code> - adds a driver to a certain car</li>
        <li>DeleteCarController - <code>GET /cars/delete</code> - deletes car</li>
        <li>GetAllCarsController - <code>GET /cars</code> - views all cars</li>
        <li>AddDriverController - <code>POST /drivers/add</code> - adds a driver</li>
        <li>DeleteDriverController - <code>GET /drivers/delete</code> - deletes driver</li>
        <li>GetAllDriversController - <code>GET /drivers</code> - views all drivers</li>
        <li>GetMyCurrentCarsController - <code>GET /drivers/cars</code> - views all cars for the current driver</li>
        <li>AddManufacturersController - <code>POST /manufacturers/add</code> - adds new manufacturer</li>
        <li>DeleteManufacturerController - <code>GET /manufacturers/delete</code> - deletes manufacturer</li>
        <li>GetAllManufacturersController - <code>GET /manufacturers</code> - views all manufacturers</li>
    </ul>
<li>dao: Data Access Object interfaces and their implementations</li> 
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
<li>Java <code>v.17.0.5</code></li>
<li>Maven <code>v.3.8.6</code></li>
<li>JDBC <code>v.4.2</code></li>
<li>MySql <code>v.8.0.24</code></li>
<li>Java Servlets <code>v.4.0.1</code></li>
<li>Tomcat <code>v.9.0.73</code></li>
</ul>

## Authors

Yehor Cherkashyn
