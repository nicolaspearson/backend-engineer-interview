## Backend Engineer Coding Challenge

This is a technical coding challenge for the backend engineering position. You have 1 week to 
complete this challenge in your own time, and we would like you to create the project on `github`.

Feel free to get in touch if you have questions regarding the assignment.

### Challenge

1. Create a RESTful API service that can perform CRUD (create / read / update / delete) operations on persisted user data.

    The user model should consist of the following:
    ```json
    {
      "id": 1,                  // the unique identifier of the record
      "firstName": "",          // the first name of the user
      "lastName": "",           // the last name of the user
      "email": "",              // the email address of the user
      "dateOfBirth": "",        // the date of birth of the user
      "address": "",            // the physical address of the user 
      "createdAt": "",          // the date the record was created
      "updatedAt": ""           // the date the record was updated
    }
    ```

2. Create a github action that runs the tests and builds the application if the tests pass.

    **Bonus**: Bundle the application and include it in a docker image as a step in pipeline (the application in the image does not need to connect to an external database).

### Requirements:

1. Programming language:
    - You may use any popular backend programming language to complete the challenge, e.g. Python, Typescript, Javascript, Java, C#, Ruby, Rust, Go, etc.
2. API design:
    - The RESTful API design should follow best practices.
2. Data modelling:
    - You may using any suitable data storage technique / database technology (RDBMS / NOSQL) (e.g. PostgreSQL, MySQL, MongoDB etc.).
3. Testing:
    - Ideally you should provide unit tests for your code. Integration tests would be a bonus.
4. CI automation:
    - CI automation should be done using Github action(s).
5. Docker
    - A `DockerFile` should be created for the application. 
    - A `docker-compose.yaml` file should be created for the application, and any external dependencies, e.g. a database.
6. Documentation
    - At a minimum you should provide documentation that explains what the application does, how to run it, and how to run the tests.

### What We Review

The aspects of your code we will judge include:

- **Clarity**: Does the README clearly explain the application and how it works?
- **Correctness**: Does the application do what was asked? If there is anything missing, does the README explain why it is missing?
- **Code** Quality: Is the code simple, easy to understand, and maintainable?
- **Testing**: How thorough are the automated tests? Will they be difficult to change if the requirements of the application were to change?
- **Technical Choices**: Do the choices of libraries / databases / architecture seem appropriate for the challenge?
