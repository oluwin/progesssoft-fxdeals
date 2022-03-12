# ProgressSoft FxDeals for Bloomberg (Demo)
This is a demo application that uploads, analyses and persists FX Deals in the DB.


# Technology & Dependencies
- MySql 8.0
- Jdk 11
- Intellij IDE
- Spring Boot 2.6.4 (with Spring Web MVC)
- Maven 3.8.3
- Apache POI 5.2.0
- Postman 


# Set Up and Installation
- Download and Install jdk 8 or 11 or higher from [Oracle Site](https://www.oracle.com/java/technologies/downloads/) if you haven't
- Download and install Maven if you haven't from [here](https://maven.apache.org/download.cgi)
- Set up path variables in your system environment variables if you haven't
- Open cmd and type <kbd>java -version</kbd> and enter to confirm Java is already set up on your machine
- Type <kbd>mvn -version</kbd> and enter to confirm Maven is set up on your machine
- Use any SpringBoot template generator such as [Spring Initializr](https://start.spring.io/) which is available online to bootstrap the project. You can also use your development tool such as Spring Tool Suite, Eclipse, Intellij etc
- Launch MySQL and create a Database.


# Usage
- Clone this repository to your local machine
- Create a Dummy Excel sheet. Make sure you rename default Sheet 1 to whatever you have changed it to in the excel reader package.(A dummy file has been attached to this project)
- Import the project into Intellij IDE or any of your desirable IDE
- Modify the properties file to match your connection and port settings
- Run the application
- Once the application is running, go to postman and send a post request to upload the excel sheet (In the Request body, check the box and select file under key, type 'file' in the field provided and select the excel sheet under value column)
- Once the above is set, you may send the request and wait for a response. If upload is successful or not, you will get a response.
- Check MySql Database to confirm. Spring automatically creates the tables and columns as specified in the Model class.
- You can clone the Containerized version [here](https://github.com/oluwin/progress-soft-fxdeals-docker-compose)


# Contributing
Pull requests are welcome. For major changes, please open an issue first to discuss what you would like to change.
Please make sure to update tests as appropriate.
