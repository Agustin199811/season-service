# Season Service for E-commerce Application

This project is a Season Service for an e-commerce clothing application. The Season Service is designed to manage clothing seasons, allowing other microservices within the platform to effectively interact with season data. By centralizing season management, it ensures consistency and accuracy in the representation of clothing seasons across the e-commerce platform.

## Table of Contents

- [Overview](#overview)
- [Features](#features)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Configuration](#configuration)
- [Running the Service](#running-the-service)
- [Contributing](#contributing)
- [License](#license)

## Overview

The Season Service is a RESTful API built using Spring Boot. It provides endpoints for creating, updating, retrieving, and deleting clothing seasons. This service plays a crucial role in the product management system by ensuring that season data is uniformly managed and easily accessible to other microservices.

## Features

- **Create Seasons:** Allows the creation of new clothing seasons with detailed descriptions.
- **Retrieve Seasons:** Enables fetching details of existing seasons, supporting features like product filtering and search.

## Prerequisites

- Java 17 or higher
- Maven 3.6.3 or higher
- Spring Boot 3 or higher

## Installation

1. Clone the repository:

    - ```sh
      git clone https://github.com/Agustin199811/season-service.git
      cd season-service
      ```

2. Build the project using Maven:

    - ```sh
      mvn clean install
      ```

## Configuration

The configuration for the Season Service is located in `src/main/resources/application.properties`. Below is an example configuration:

```properties
spring.datasource.url=jdbc:postgresql://clot-postgreasql.cp88o8squjfi.us-east-1.rds.amazonaws.com:5432/clot
spring.datasource.username=postgres
spring.datasource.password=root1234

eureka.client.service-url.defaultZone=http://clot-ecommerce-ELB-1792240696.us-east-1.elb.amazonaws.com:8761/eureka/
eureka.client.register-with-eureka=true
eureka.client.fetch-registry=true
```

## Running the Service

To run the service registry, use the following command:

 ```sh
    mvn spring-boot:run
```

## Contributing

Contributions are welcome! If you would like to contribute to this project, please send us an email at
`toapantaagustin9c@gmail.com` with details about your proposed changes or improvements. We look forward to hearing from you!

## License

This project is licensed under the MIT License - see the LICENSE file for details.
