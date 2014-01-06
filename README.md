Spring MVC 4 Quickstart Maven Archetype=========================================Summary-------The project is a Maven archetype for Spring MVC 4 web application. Used by Cody IT Solutios to kickstart his applications.Generated project characteristics-------------------------* No-xml Spring MVC 4 web application for Servlet 3.0 environment* Thymeleaf as template engine.* JPA 2.1 (Hibernate/HSQLDB or MySQL/Spring Data JPA)* JUnit/Mockito* Spring Security 3.2* Logback for logging* Uses [Bower](http://bower.io/) on client side as package manager with [Bootstrap 3 for Sass](http://getbootstrap.com/), [jQuery](http://jquery.com/), [AngularJS](http://angularjs.org/) as dependencies.* Supports Internationalization (i18n)Future Features------------* Add Grunt as client side task runner.* Add Production and Testing profiles to pom.xml* Installation------------run `mvn clean install` to install the archetype in your local repositoryCreate a project----------------    mvn archetype:generate \        -DarchetypeGroupId=com.github.spring-mvc-archetypes \        -DarchetypeArtifactId=spring-mvc-quickstart \        -DarchetypeVersion=1.0.0-SNAPSHOT \        -DgroupId=my.groupid \        -DartifactId=my-artifactId \        -Dversion=versionRun the project----------------		mvn test tomcat7:runNote: No additional services are required in order to start the application. Mongo DB configuration is in place but it is not used in the code.Creating a new project in Eclipse----------------------------------* Install the archetype in local repository with `mvn install`* Go to `Preferences > Maven > Archetypes` and `Add Local Catalog`* Select the catalog from file (`archetype-catalog.xml`) * Create new Maven project and select the archetype (remember so select `Include snapshot archetypes`).Thanks to [kolorobot](https://github.com/kolorobot) for starting this archetype.