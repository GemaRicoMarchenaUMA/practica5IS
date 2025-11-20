# Copilot Instructions for practica5

## Project Overview
This is a Java Spring Boot application located in `src/main/java/com/GrupoG/practica5/`. The main entry point is `Practica5Application.java`. The project follows standard Spring Boot conventions for structure and configuration.

## Architecture & Structure
- **Main Application:** `Practica5Application.java` is the starting point. Additional components, services, or controllers should be placed in the same package or subpackages.
- **Resources:** Configuration and static assets are in `src/main/resources/`.
  - `application.properties` for app config.
  - `static/` for web assets.
  - `templates/` for server-side templates.
- **Tests:** Unit and integration tests are in `src/test/java/com/GrupoG/practica5/`.

## Developer Workflows
- **Build:** Use Maven wrapper scripts (`mvnw` or `mvnw.cmd`) for building and running the project.
  - Example: `./mvnw clean install` (Linux/macOS) or `mvnw.cmd clean install` (Windows PowerShell)
- **Run:** Start the app with `./mvnw spring-boot:run` or `mvnw.cmd spring-boot:run`.
- **Test:** Run tests with `./mvnw test` or `mvnw.cmd test`.

## Patterns & Conventions
- **Package Naming:** All source code is under `com.GrupoG.practica5`.
- **Spring Boot:** Use annotations like `@SpringBootApplication`, `@RestController`, `@Service`, and `@Repository` for component roles.
- **Configuration:** Place all config in `application.properties`.
- **Static/Template Files:** Use `resources/static` and `resources/templates` for web assets and views.

## Integration Points
- **External Dependencies:** Managed via Maven in `pom.xml`.
- **Spring Boot:** Handles dependency injection, web server, and configuration.

## Examples
- To add a REST endpoint, create a class in `com.GrupoG.practica5` and annotate with `@RestController`.
- To add a service, use `@Service` and inject it into controllers.

## Key Files
- `src/main/java/com/GrupoG/practica5/Practica5Application.java`: Main class.
- `src/main/resources/application.properties`: Configuration.
- `pom.xml`: Dependency management.
- `src/test/java/com/GrupoG/practica5/Practica5ApplicationTests.java`: Example test.

---
**For AI agents:**
- Follow Spring Boot conventions unless project files indicate otherwise.
- Use Maven wrapper scripts for all build/run/test commands.
- Place new code in the appropriate package and directory.
- Reference `pom.xml` for dependencies.
