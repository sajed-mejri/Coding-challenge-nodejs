# VISI-ONE Coding challenge

Welcome! Thank you for taking the time to apply.  We value your time, so please limit yourself to 90 minutes for the solution.  This keeps it fair for everyone.

The API has been built with Node.js, Express, SQLite, and Knex.js.  We would like you to improve a few things.

## Things to Improve

- Refactor the Express API handlers to follow best practices and maintainability.
- Write unit tests for the Express API handlers using a testing framework of your choice.
- Add a Dockerfile for the project and provide commands to build and run the application inside a Docker container. Ensure ports are properly exposed.
- Create a migration for a new entity, "vehicles" and add an endpoint to retrieve vehicles.
- Add an endpoint that allows the pairing of a vehicle with a priceboard, but only if the priceboard and vehicle belong to the same tenant.

## Setup

1. Clone the project:

   ```bash
   git clone <repository_url>
   cd Coding-challenge-nodejs
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

3. Initialize the database and seed data:

   ```bash
   make init-db
   ```

4. Start the Express app:

   ```bash
   make start
   ```

The API will be accessible at `http://localhost:3000`.

## Database Migrations and Seeding

- Database migrations and seeding are managed using Knex.js. To create new migrations and seed data, use the following commands:

   - Create a new migration:
     ```bash
     npx knex migrate:make migration_name
     ```

   - Run migrations:
     ```bash
     npx knex migrate:latest
     ```

   - Create a new seed file:
     ```bash
     npx knex seed:make seed_name
     ```

   - Run seed data:
     ```bash
     npx knex seed:run
     ```

## Collaborating

1. Fork this repository to your own GitHub account.

2. Clone your forked repository and make changes as needed.

3. Create a new branch for your changes:

   ```bash
   git checkout -b your-name/your-branch-name
   ```

4. Commit your changes and push to your GitHub repository:

   ```bash
   git add .
   git commit -m "Add your commit message here"
   git push origin your-name/your-branch-name
   ```

5. Create a Pull Request (PR) from your repository to the original project's repository.

6. The project owner will review your PR and provide feedback. Please be patient, we will try to send feedback within a week.

## Postman Collection

Please create and include a Postman collection in the project that calls the endpoints. This will facilitate testing and documentation of the API.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.