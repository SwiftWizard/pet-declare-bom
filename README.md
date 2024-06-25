# DECLARE-PET PROJECT BOM (Bill of Materials)

* Used to store a single maven pom file that contains common dependencies used in DeclarePet microservices
* Makes dependency management easier

# Goals

* One configuration across multiple services using same dependency version
* Make changes in one place, not multiple ones

# Change log

* Initial commit:
  * Declared "spring-boot-starter-parent" as the parent pom - to inherit is dependencies and configs into the BOM
  * Setup group, version, version
  * Defined license
  * Organization and developer
  * Common properties, such as Java, Lombok, Mapstruct.. versions and targets, 
  * DependencyManagement to declare versions of dependencies to be used - only once
  * Mapstruct-Lombok configuration
  * Plugins: maven-clean, maven-enforcer-plugin for min Java and Maven versions
