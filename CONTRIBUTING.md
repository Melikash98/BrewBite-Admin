# Contributing to BrewBite Admin Backend

Thank you for your interest in contributing to **BrewBite Admin Backend**.

This project powers the admin side of the BrewBite café & bakery platform. Contributions are welcome as long as they are consistent with the project structure, code style, and security expectations.

## How to Contribute

### 1. Open an Issue First
Before starting work on a new feature or fix, please open an issue to describe:
- the problem you found,
- the feature you want to add,
- or the improvement you are proposing.

This helps avoid duplicate work and keeps the project direction clear.

### 2. Fork and Clone the Repository
Fork the repository to your GitHub account, then clone your fork locally:

```bash
git clone https://github.com/<your-username>/BrewBite-Admin.git
cd BrewBite-Admin
```

### 3. Create a Feature Branch
Use a descriptive branch name:

```bash
git checkout -b feature/order-status-improvement
git checkout -b fix/jwt-validation-bug
git checkout -b docs/update-readme
```

### 4. Set Up the Project Locally
Make sure you have the required environment before making changes.

#### Prerequisites
- Java 17 or higher
- Maven
- PostgreSQL
- Cloudinary account
- IDE such as IntelliJ IDEA or Eclipse

#### Local Configuration
Update `application.properties` with your local credentials:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/brewbite_admin
spring.datasource.username=YOUR_DB_USERNAME
spring.datasource.password=YOUR_DB_PASSWORD
spring.jpa.hibernate.ddl-auto=update

jwt.secret=YOUR_JWT_SECRET_KEY
jwt.expiration=86400000

cloudinary.cloud-name=YOUR_CLOUD_NAME
cloudinary.api-key=YOUR_API_KEY
cloudinary.api-secret=YOUR_API_SECRET
```

Then run the application:

```bash
./mvnw spring-boot:run
```

## Code Standards

Please follow these rules when contributing:

### Java Code Style
- Use clear and meaningful class, method, and variable names.
- Keep methods short and focused on a single responsibility.
- Follow standard Java naming conventions.
- Prefer constructor injection over field injection.
- Keep controllers thin and business logic inside services.
- Keep repository logic limited to data access.
- Reuse existing helpers, mappers, and exception handlers where possible.

### Spring Boot Best Practices
- Keep layers separated:
  - `controller` for HTTP endpoints
  - `service` for business logic
  - `repository` for persistence
  - `entity` for database models
  - `dto` for request/response objects
- Validate all user input.
- Return consistent API responses.
- Do not expose sensitive data in responses.
- Preserve the existing security rules and role-based access control.

### Formatting
- Use consistent indentation.
- Avoid unnecessary comments.
- Keep imports clean and remove unused ones.
- Format code before submitting.

## Testing

All contributions should be tested before opening a pull request.

### What to Test
- API endpoints
- validation rules
- authentication and authorization
- order flow
- database interactions
- edge cases and error handling

### Running Tests
If tests exist in the project, run them before submitting:

```bash
./mvnw test
```

If you add new functionality, include tests whenever possible.

## Commit Guidelines

Use clear and descriptive commit messages.

Examples:
```bash
git commit -m "Add order status update endpoint"
git commit -m "Fix JWT validation error"
git commit -m "Refactor complaint service logic"
git commit -m "Update API documentation"
```

Keep each commit focused on one logical change.

## Pull Request Guidelines

Before opening a pull request, make sure:
- your code is complete and working,
- tests pass locally,
- your branch is up to date with the latest main branch,
- your changes are described clearly,
- any related issue is linked.

### Pull Request Checklist
- [ ] Code follows the project structure
- [ ] Code is formatted and clean
- [ ] Tests have been run
- [ ] No sensitive values are committed
- [ ] API documentation is updated if needed
- [ ] Changes are explained clearly in the PR description

## Reporting Bugs

When reporting a bug, please include:
- a clear title,
- steps to reproduce,
- expected result,
- actual result,
- screenshots or logs if available,
- your environment details if relevant.

## Suggesting Features

When suggesting a feature, please explain:
- the problem it solves,
- why it is useful,
- how it fits into the current system,
- any possible implementation ideas.

## Security

Security-related changes are especially important in this project.

Please do not:
- commit passwords, secrets, or API keys,
- weaken authentication or authorization checks,
- bypass validation,
- expose private business data.

If you discover a security issue, report it responsibly through an issue or private communication method if one is available.

## Project Areas You May Contribute To

Typical contribution areas include:
- authentication and authorization
- item and category management
- order management
- revenue and reporting
- ratings and reviews
- comments and replies
- complaint handling
- analytics and dashboard improvements
- API documentation
- bug fixes and refactoring

## License

By contributing to this repository, you agree that your contributions will be licensed under the same license as the project.

---

Thank you for helping improve BrewBite Admin Backend.
