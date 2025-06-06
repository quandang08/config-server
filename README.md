Config Server (Native Mode) in Microservices Architecture

* Overview
The Config Server in native mode provides centralized configuration management for microservices by retrieving configuration files from the local file system instead of external sources like Git or SVN.


* How It Works in Microservices
Centralized Configuration: Config Server stores configurations in one place, allowing all microservices to retrieve them.

* Microservice Requests: Microservices make HTTP requests to the Config Server to fetch configuration properties specific to their service, environment, and profile (e.g., GET http://localhost:8888/user-service/dev/main).

* Native Mode: Configurations are stored in the local file system (classpath:/configurations) and are served when requested.

* Benefits in Microservices
Consistency: Centralized configuration for all microservices, ensuring consistency across the system.

Ease of Management: Simplifies updates and maintenance of configuration files without altering individual microservices.
