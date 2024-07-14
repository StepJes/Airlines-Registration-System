# Airlines Registration System

<p align="center">
  <img src="https://raw.githubusercontent.com/StepJes/Airlines-Registration-System/main/banner.jpg" alt="Smart Contact Manager">
</p>

This is an Airlines Registration System created using Java and the Struts 1 framework.

## Features

* User Registration and Authentication
* Flight Booking and Cancellation
* Search for Flights by Destination and Date
* View Booking History
* REST API for flight and booking management
* Modern UI with JavaScript and AJAX

## Prerequisites

Be sure you have the following installed on your development machine:

+ Java Development Kit (JDK) >= 8
+ PostgreSQL
+ Maven
+ Git
+ Postman

## Project Installation

To setup a local development environment:

Clone the GitHub Project,
```bash
git clone git@github.com:StepJes/Airlines-Registration-System.git

cd Airlines-Registration-System
```

Install project dependencies,
```bash
mvn install
```

Configure the database:

1. Create a PostgreSQL database named `airlines_registration_system`.
2. Update the `src/main/resources/application.properties` file with your PostgreSQL credentials.
   ```properties
   spring.datasource.url=jdbc:postgresql://localhost:5432/airlines_registration_system
   spring.datasource.username=<your_postgresql_username>
   spring.datasource.password=<your_postgresql_password>
   spring.jpa.hibernate.ddl-auto=update
   ```

Run the application,
```bash
mvn jetty:run
```

The application will be available at `http://localhost:8080`.

## API Testing with Postman

1. Import the provided Postman collection `Airlines-Registration-System.postman_collection.json` into Postman.
2. Use the collection to test the REST API endpoints for flight and booking management.

## Features in Detail

### User Registration and Authentication
- Users can register for an account, log in, and manage their profile.

### Flight Booking and Cancellation
- Users can book flights and cancel bookings through the system.

### Search for Flights
- Users can search for available flights by destination and date.

### View Booking History
- Users can view their past bookings and transaction history.

### Payment Processing
- The system includes a payment processing feature to handle flight bookings.

### REST API
- The application exposes RESTful endpoints for managing flights and bookings programmatically.

## Technologies Used

- **Backend**: Java, Struts 1, REST API
- **Frontend**: JavaScript, AJAX, HTML, CSS
- **Database**: PostgreSQL
- **API Testing**: Postman
- **Build Tool**: Maven

## Conclusion

The Airlines Registration System is designed to streamline the process of booking and managing flights. Using Java and Struts 1 for the backend provides a robust framework, while JavaScript and AJAX enhance the user experience on the frontend. The integration of REST APIs allows for flexible interaction with the system, and PostgreSQL ensures reliable data storage. Postman is utilized for thorough API testing, making this a comprehensive solution for airline registration and booking needs.
