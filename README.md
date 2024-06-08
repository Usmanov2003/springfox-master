For more information on this project visit the Springfox Website or http://springfox.github.io/springfox/

Useful links
Reference Documentation
Examples repository
Contribution Guidelines
Core contributors
Development and contribution guidelines
Change log
Development Environment
Release Instructions
Getting Started
For new projects
For Maven

<dependency>
    <groupId>io.springfox</groupId>
    <artifactId>springfox-boot-starter</artifactId>
    <version>3.0.0</version>
</dependency>
For Gradle

  implementation "io.springfox:springfox-boot-starter:<version>"
Migrating from earlier snapshot
Spring Boot Applications
NOTE: Would love feedback to make this better

Remove explicit dependencies on springfox-swagger2
Remove any @EnableSwagger2... annotations
Add the springfox-boot-starter dependency
Springfox 3.x removes dependencies on guava and other 3rd party libraries (not zero dep yet! depends on spring plugin and open api libraries for annotations and models) so if you used guava predicates/functions those will need to transition to java 8 function interfaces.
Migrating from existing 2.x version
Spring Boot Applications
NOTE: Would love feedback to make this better

Remove explicit dependencies on springfox-swagger2
Remove the @EnableSwagger2 annotations
Add the springfox-boot-starter dependency
Springfox 3.x removes dependencies on guava and other 3rd party libraries (not zero dep yet! depends on spring plugin and open api libraries for annotations and models) so if you used guava predicates/functions those will need to transition to java 8 function interfaces
If you are using WebMvc but you don't use the @EnableWebMvc annotation yet, add this annotation.
Regular spring mvc
NOTE: Would love feedback to make this experience better

Remove explicit dependencies on springfox-swagger2
Add @EnableOpenApi for open API (and @EnableSwagger2WebMvc or @EnableSwagger2WebFlux for older versions)
Added the springfox-oas library
Springfox 3.x removes dependencies on guava and other 3rd party libraries (not zero dep yet! depends on spring plugin and open api libraries for annotations and models) so if you used guava predicates/functions those will need to transition to java 8 function interfaces
