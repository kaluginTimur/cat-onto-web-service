# cat-onto-web-service

**Archivation Notice:** This project is an old student project and is no longer actively maintained. It is provided for historical reference or educational purposes only.

## Project Description

This project is a Java web application that served as a demonstration or exploration of ontological concepts, using the OWLAPI library for working with ontologies. It is a Spring MVC application, serving JSP pages.

It provides web services and a web interface to interact with information related to cat breeds characteristics based on an underlying ontology.

## Technologies Used

*   **Backend:** Java, Spring MVC
*   **Ontology Processing:** OWLAPI (Open Web Ontology Language API)
*   **Web Server:** Servlet API (deployed on a Java EE compatible server like Tomcat)
*   **Frontend:** JSP, JSTL, HTML, CSS, JavaScript
*   **Build Tool:** Apache Maven

## Setup and Running

1.  **Prerequisites:**
    *   Java Development Kit (JDK) 8
    *   Apache Maven
    *   A Servlet container (e.g., Apache Tomcat)

2.  **Build:**
    ```bash
    mvn clean install
    ```
    This command compiles the project, runs tests, and packages the application into a `.war` file in the `target/` directory.

3.  **Deployment:**
    Deploy the generated `.war` file (e.g., `catOntoWebService-1.0-SNAPSHOT.war`) to your Servlet container (e.g., by copying it to Tomcat's `webapps` directory).

4.  **Access:**
    Once deployed and the server is running, you should be able to access the application in your web browser, typically at `http://localhost:8080/catOntoWebService/` (the exact URL might vary depending on your server configuration and the context root).

## Project Structure Highlights

*   `src/main/java`: Contains the Java source code, including Spring controllers (`MainController.java`), semantic processing logic (`OntologyProcessor.java`, `OntologyUtil.java`), and ontology vocabulary (`Catonto.java`).
*   `src/main/resources/semantic/ontology`: Contains the OWL ontology file (`catonto.owl`) and its catalog.
*   `src/main/webapp`: Contains web resources like JSP pages (`index.jsp`, `breeds.jsp`, `breedInfo.jsp`), CSS, JavaScript, and images.
*   `pom.xml`: Maven project configuration file.
