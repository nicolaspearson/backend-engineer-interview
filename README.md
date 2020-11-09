## Backend Engineer Technical Challenge

This is a technical coding challenge for the backend engineering position. You have 1 week to 
complete this challenge in your own time, and we would like you to create the project on `github`.

Feel free to get in touch if you have questions regarding the assignment.

### Application

Create a Node.js application that provides the following functionality:

1. A user should be able to register, by providing the following profile information:
- First name
- Last name
- Email address
- Physical address (street and house number, postal code, city)
- Password
2. A user should be able to login using their email address and password, and the server should return a JWT.
3. A user should be able to retrieve their own profile by providing the JWT in the request.
4. A user should be able to update their information by providing a JWT and one or more of the following fields:
- First name
- Last name
- Email address
- Physical address (street and house number, postal code, city)
5. A user should be able to change their password by providing the JWT in the request, their existing password, and the new password.

**Bonus**: We appreciate good documentation this can be done via: 
- The `README` in the project root.
- `TSDoc` comments in your code.
- Using Swagger to document the API.

### Requirements:

The aim of this coding challenge is to assess the following competencies:
1. Node.js:
- You may use a Node.js framework (e.g. [NestJS](https://nestjs.com/)).
2. Typescript:
- The source code must be written in Typescript.
3. Database:
- You may using any suitable database technology (RDBMS / NOSQL) (e.g. PostgreSQL, MySQL, MongoDB etc.).
4. Testing:
- You should write both unit tests and integration tests for the source code using Jest or an equivalent technology.
5. CI automation:
- CI automation should be done via a Github action(s).
6. Docker
- A `DockerFile` should be created for the application. 
- A `docker-compose.yaml` file should be created for the application, and any external dependencies, e.g. the database.

You may use `yarn` / `npm` as the package manager for the project.

### Scripts:

You should have the following scripts in your `package.json` file:
- Build the application, e.g. `yarn build`
- Start the application in development mode along with any external dependencies, e.g. `yarn start:dev`
- Start the application in production mode (excluding external dependencies), e.g. `yarn start:prod`
- Run the unit tests, e.g. `yarn test:unit`
- Run the integration tests, e.g. `yarn test:integration`

### CI Automation:

Create a github action that runs the tests and builds the application if the tests pass.

**Bonus**: Bundle the application and include it in a docker image as a step in pipeline (the application in the image does not need to connect to an external database).
