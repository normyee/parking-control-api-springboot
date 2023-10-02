# Parking Control API

The Parking Spot API is a Spring Boot project designed to manage parking spot information. It follows the Model-View-Controller (MVC) architecture, with the use of repositories and DTOs for request validation. The project utilizes PostgreSQL as its database.

## Project Overview

- **MVC Architecture:** The project follows the Model-View-Controller architectural pattern to separate concerns and maintain a structured codebase.

- **Repositories:** Repositories are used to interact with the PostgreSQL database. They provide data access and manipulation methods for the application.

- **DTOs for Request Validation:** Data Transfer Objects (DTOs) are employed to validate and structure incoming requests, ensuring data integrity and security.

## Database Configuration

The application is configured to use PostgreSQL as its database. Make sure you have a PostgreSQL database set up, and configure the database connection in the `application.properties` or `application.yml` file.

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/parking_spot_db
spring.datasource.username=your_username
spring.datasource.password=your_password
```

# API Endpoints
The API endpoints are accessible at the following base URL:
```
http://localhost:8080/parking-spot
```

To perform CRUD (Create, Read, Update, Delete) operations on parking spots, you can use different HTTP methods:

* Create a new parking spot: POST /parking-spot
* Retrieve all parking spots: GET /parking-spot
* Retrieve a specific parking spot: GET /parking-spot/{id}
* Update a parking spot: PUT /parking-spot/{id}
* Delete a parking spot: DELETE /parking-spot/{id}<br/><br/>

Please make sure to adapt the HTTP method and endpoint as needed for your specific operation.
