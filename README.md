[![Build Status](https://travis-ci.org/Relesi/ponto-inteligente-api-1.1.svg?branch=master)](https://travis-ci.org/Relesi/ponto-inteligente-api-1.1)
# Eureka-Server

Store for integration system with Java and Spring Boot.

### RESTful API details

#### Features

* Service Discovery: Eureka instances can be registered and clients can discover the instances using Spring-managed beans
* Service Discovery: an embedded Eureka server can be created with declarative Java configuration
* Circuit Breaker: Hystrix clients can be built with a simple annotation-driven method decorator
* Circuit Breaker: embedded Hystrix dashboard with declarative Java configuration
* Client Side Load Balancer: Ribbon
* External Configuration: a bridge from the Spring Environment to Archaius (enables native configuration of Netflix components using Spring Boot conventions)
* Router and Filter: automatic registration of Zuul filters, and a simple convention over configuration approach to reverse proxy creation

### Modules In Maintenance Mode

Placing a module in maintenance mode means that the Spring Cloud team will no longer be adding new features to the module.
We will fix blocker bugs and security issues, and we will also consider and review small pull requests from the community.

We intend to continue to support these modules for a period of at least a year from the general availability
of the Greenwich release train.

The following Spring Cloud Netflix modules and corresponding starters will be placed into maintenance mode:

* spring-cloud-netflix-archaius
* spring-cloud-netflix-concurrency-limits
* spring-cloud-netflix-hystrix-contract
* spring-cloud-netflix-hystrix-dashboard
* spring-cloud-netflix-hystrix-stream
* spring-cloud-netflix-hystrix
* spring-cloud-netflix-ribbon
* spring-cloud-netflix-turbine-stream
* spring-cloud-netflix-turbine
* spring-cloud-netflix-zuul

NOTE: This does not include the Eureka modules.


#### Building

	:jdkversion: 1.8

#### Basic Compile and Test

To build the source you will need to install JDK {jdkversion}.

Spring Cloud uses Maven for most build-related activities, and you
should be able to get off the ground quite quickly by cloning the
project you are interested in and typing


	$ ./mvnw install


----
### How to run the service

	Make sure you have Maven installed and added to your operating system's PATH, as well as Git.
	cd /path/to/your/repo
	mvn spring-boot:run
	
### Importing the project into Eclipse STS, Eclipse or Intellij

mvn eclipse:eclipse

In STS/Eclipse import the project as project Maven.

After the project is imported, change the application to test and run the following commands.

mvn clean install

mvn install

maven - update project
