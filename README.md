# Address Book (Spring Boot)

## Overview

Create a RESTful API using **Spring Boot**, **Java**, and **Hibernate/JPA**, following industry-recognized standards and best practices.

The API should allow clients to view, search, and edit the contact database. You will utilize an **H2 in-memory database**; the database configuration and sample data are provided.

---

## Details

### Endpoints

Create endpoints that do each of the following things. You should decide appropriate naming and methods.

- List all contacts, with options for pagination and sorting.
  - *Example: Get the page 2 of 10 contacts, sorted by lastName in descending order.*
- View details for a specific contact.
  - *Example: Retrieve the contact with ID 5.*
- Create a new contact. Return the created contact with its assigned ID.
- Update an existing contact.
- Delete a contact.
- Search contacts by name, email, city, or state. Support pagination and sorting on results.
  - *Example: Search for "smith", return page 1 with 5 results, sorted by city ascending.*

### Database

The H2 database is pre-configured with sample data. The `contacts` table has these columns:

- id
- first_name
- last_name
- street
- city
- state
- zip
- phone
- email

### What's Provided

- `pom.xml` - Maven build file with Spring Boot, JPA, H2, and Validation dependencies
- `application.properties` - H2 database configuration (ready to use)
- `schema.sql` - Creates the contacts table on startup
- `data.sql` - Seeds 15 sample contacts
- `AddressBookApplication.java` - Spring Boot entry point

### Running the Application

```bash
mvn spring-boot:run
```

The API will be available at `http://localhost:8080`

The H2 Console (for debugging) is available at `http://localhost:8080/h2-console`:
- JDBC URL: `jdbc:h2:mem:addressbook`
- Username: `sa`
- Password: *(leave empty)*

### Documentation/API Client

You do not need to create a front end. Optionally, you can create tests or Postman/Bruno collections to show your API's operation. As an alternative, at least provide some documentation in a README so we know how to make requests.

---

## Preparing for the Interview

**[Next Steps...](../../next-steps-real-time.md)**
