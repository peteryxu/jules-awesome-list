<p align="center">
  <img src="assets/jules-readme.png" alt="Jules Awesome List" width="600">
</p>

<div align="center">
  <h1>Awesome Jules Prompts 🌟</h1>
  <p>Curated prompts for Jules, an async coding agent from Google Labs.</p>
  <br>
  <a href="https://jules.google.com">Visit Jules</a> •
  <a href="#contributing">Contribute</a>
</div>

---

## Table of Contents

- [Table of Contents](#table-of-contents)
- [Everyday Dev Tasks](#everyday-dev-tasks)
- [Debugging](#debugging)
- [Documentation](#documentation)
- [Testing](#testing)
  - [Test Data Generation](#test-data-generation)
  - [Test Strategy & Planning](#test-strategy--planning)
- [Package Management](#package-management)
- [Security & Compliance](#security--compliance)
- [AI-Native Tasks](#ai-native-tasks)
- [Code Transformation & Modernization](#code-transformation--modernization)
- [Context](#context)
- [Fun & Experimental](#fun--experimental)
- [Start from Scratch](#start-from-scratch)
- [Contributing](#contributing)

---

## Everyday Dev Tasks

- `// Refactor {a specific} file from {x} to {y}...`
  <sub>General-purpose, applies to any language or repo.</sub>

- `// Add a test suite...`
  <sub>Useful for repos lacking test coverage.</sub>

- `// Add type hints to {a specific} Python function...`
  <sub>Python codebases transitioning to typed code.</sub>

- `// Generate mock data for {a specific} schema...`
  <sub>APIs, frontends, or test-heavy environments.</sub>

- `// Convert these commonJS modules to ES modules...`
  <sub>JS/TS projects modernizing legacy code.</sub>

- `// Turn this callback-based code into async/await...`
  <sub>JavaScript or Python codebases improving async logic.</sub>

- `// Implement a data class for this dictionary structure...`
  <sub>Useful for Python projects moving towards more structured data handling with `dataclasses` or Pydantic.</sub>



## Debugging

- `// Help me fix {a specific} error...`
  <sub>For any repo where you're stuck on a runtime or build error.</sub>

- `// Why is {this specific snippet of code} slow?`
  <sub>Performance profiling for loops, functions, or queries.</sub>

- `// Trace why this value is undefined...`
  <sub>Frontend and backend JS/TS bugs.</sub>

- `// Diagnose this memory leak...`
  <sub>Server-side apps or long-running processes.</sub>

- `// Add logging to help debug this issue...`
  <sub>Useful when troubleshooting silent failures.</sub>

- `// Find race conditions in this async code`
  <sub>Concurrent systems in JS, Python, Go, etc.</sub>

- `// Add print statements to trace the execution flow of this Python script...`
  <sub>For debugging complex Python scripts or understanding unexpected behavior.</sub>


## Documentation

- `// Write a README for this project`
  <sub>Any repo lacking a basic project overview.</sub>

- `// Add comments to this code`
  <sub>Improves maintainability of complex logic.</sub>

- `// Write API docs for this endpoint`
  <sub>REST or GraphQL backends.</sub>

- `// Generate Sphinx-style docstrings for this Python module/class/function...`
  <sub>Ideal for Python projects using Sphinx for documentation generation.</sub>



## Testing

- `// Add integration tests for this API endpoint`
  <sub>Express, FastAPI, Django, Flask apps.</sub>

- `// Write a test that mocks fetch`
  <sub>Browser-side fetch or axios logic.</sub>

- `// Convert this test from Mocha to Jest`
  <sub>JS test suite migrations.</sub>

- `// Generate property-based tests for this function`
  <sub>Functional or logic-heavy code.</sub>

- `// Simulate slow network conditions in this test suite`
  <sub>Web and mobile apps.</sub>

- `// Write a test to ensure backward compatibility for this function`
  <sub>Library or SDK maintainers.</sub>

- `// Write a Pytest fixture to mock this external API call...`
  <sub>For Python projects using Pytest and needing robust mocking for testing.</sub>

### Test Data Generation

Generating diverse, realistic, and comprehensive test data is a critical yet often tedious aspect of software testing. Jules can be an invaluable assistant in this area by automating data creation, covering edge cases, helping anonymize sensitive data, and generating data for specific scenarios.

- `// Jules, I need to test a user profile API that accepts user data in JSON format. Generate 10 valid JSON objects representing user profiles. Each object should include fields: userId (integer, unique), username (string, 5-15 alphanumeric chars), email (valid email format), dateOfBirth (YYYY-MM-DD format, user must be at least 18 years old), and isActive (boolean). Also, generate 3 invalid JSON objects: one with a missing required field, one with an invalid email, and one where the user is underage.`
  <sub>Showcases: Generating valid and invalid data, data constraints, specific formats.</sub>
- `// My application processes product information from a CSV file. The CSV has columns: product_id, product_name, category, price, stock_quantity. Generate a sample CSV file with 20 realistic entries. Ensure price is a positive float, stock_quantity is a non-negative integer, and category is one of 'Electronics', 'Books', 'Clothing', or 'Home Goods'. Include some products with zero stock.`
  <sub>Showcases: Generating data in a specific file format (CSV), realistic data variety, and boundary conditions (zero stock).</sub>
- `// Jules, I need to populate a database table named orders for testing. The table has columns: order_id (INT, PK, auto-increment), customer_id (INT), order_date (DATETIME), total_amount (DECIMAL(10,2)), status (VARCHAR(50) - e.g., 'Pending', 'Shipped', 'Delivered', 'Cancelled'). Generate 15 SQL INSERT statements for this table with varied and realistic order data for 5 different customers, ensuring order dates are within the last 6 months and statuses are appropriately distributed.`
  <sub>Showcases: Generating SQL insert statements, relational data considerations, date ranges, and enum-like field values.</sub>

### Test Strategy & Planning

Effective testing goes beyond just writing test cases; it requires a thoughtful strategy and plan. While Jules cannot replace experienced test architects, it can significantly assist in brainstorming test scenarios, identifying appropriate test types, outlining basic test plans, and prioritizing test cases.

- `// Jules, we are developing a new e-commerce feature: 'Product Wishlist'. Users can add products to their wishlist, view it, remove items, and share it. Based on this feature description, help me brainstorm a list of key test scenarios we should cover. Categorize them into functional, usability, and basic negative tests.`
  <sub>Showcases: Brainstorming test scenarios from requirements, categorizing tests.</sub>
- `// Our team is about to start testing a new REST API for a social media application. This API has endpoints for user registration, login, posting messages, and retrieving a user's feed. What types of testing (e.g., functional, security, performance, usability) should we prioritize for this API? For each type, briefly explain why it's important in this context.`
  <sub>Showcases: Identifying relevant test types for a given application type (REST API) and justifying them.</sub>
- `// Jules, I need to create a basic test plan outline for a new mobile application module that allows users to upload and edit photos. Can you draft an outline including standard sections like: 1. Introduction/Scope, 2. Test Objectives, 3. Features to be Tested, 4. Features not to be Tested, 5. Test Approach, 6. Test Environment, 7. Roles & Responsibilities, 8. Schedule, 9. Deliverables, 10. Risks & Mitigation. Just provide the section headers and a brief description of what each should contain.`
  <sub>Showcases: Drafting a test plan outline, understanding standard test plan components.</sub>

---

## Package Management

- `// Upgrade my linter and autofix breaking config changes`
  <sub>JS/TS repos using ESLint or Prettier.</sub>

- `// Show me the changelog for React 19`
  <sub>Web frontend apps using React.</sub>

- `// Which dependencies can I safely remove?`
  <sub>Bloated or legacy codebases.</sub>

- `// Check if these packages are still maintained`
  <sub>Security-conscious or long-term projects.</sub>

- `// Set up Renovate or Dependabot for auto-updates`
  <sub>Best for active projects with CI/CD.</sub>

---

## Security & Compliance

In today's digital landscape, security and compliance are not just afterthoughts but foundational pillars of robust and trustworthy software. The "Security & Compliance" category for "Awesome Jules Prompts" is essential because it directly addresses these critical needs, showcasing how AI can empower developers to build more secure and compliant applications. Jules can play a crucial role in augmenting a developer's security and compliance efforts by assisting in early vulnerability detection, promoting secure coding practices, and helping navigate compliance requirements.

- `// Jules, review the following Java code snippet in UserInputHandler.java that processes user input from a web form. Identify potential security vulnerabilities, specifically looking for risks of Cross-Site Scripting (XSS) and SQL Injection. For each identified vulnerability, explain the risk and suggest specific code changes to mitigate it using prepared statements for SQL and proper output encoding for web display.`
  <sub>Showcases: Identification of common web vulnerabilities (XSS, SQLi), explanation of risks, and actionable remediation advice.</sub>
- `// My Node.js application uses the package.json file located at ./my-app/package.json. Can you analyze its dependencies and identify any known security vulnerabilities? For each vulnerable package, list the CVE identifier, severity, and suggest the minimum patched version I should upgrade to. If possible, generate the npm audit fix command or update the package.json directly.`
  <sub>Showcases: Dependency vulnerability scanning, CVE identification, and automated remediation suggestions.</sub>
- `// Jules, I need to implement robust input validation for a user registration form in my Python Flask application (./auth/routes.py). The form accepts a username, email, and password. Generate Python code snippets that validate the following: Username: alphanumeric, 5-20 characters. Email: valid email format. Password: at least 12 characters, containing uppercase, lowercase, digit, and special character. Explain how these validations help prevent common security issues like injection attacks or weak credential usage.`
  <sub>Showcases: Secure coding practices (input validation), generation of validation logic, and explanation of security benefits.</sub>
- `// Our web application needs a strong Content Security Policy (CSP) to mitigate XSS and data injection attacks. Generate a strict CSP header configuration suitable for a modern single-page application (SPA) built with React. The application loads scripts only from its own domain and uses inline styles. It also needs to allow images from *.cdn.example.com and connect to APIs at api.example.com. Explain each directive in the generated CSP.`
  <sub>Showcases: Generation of security configurations (CSP), understanding of security headers, and customization for specific application needs.</sub>
- `// Jules, my team is working towards GDPR compliance for our application. The module UserProfileService.java handles user profile data, including PII. Review this module and highlight areas where we might need to implement specific GDPR principles, such as data minimization, purpose limitation, and the right to erasure. (Disclaimer: I understand you are an AI and not a legal expert, but I'm looking for code-level suggestions based on common interpretations of these principles).`
  <sub>Showcases: Guidance on compliance (with disclaimer), identifying PII handling, and suggesting code adjustments related to privacy principles.</sub>

---

## AI-Native Tasks

- `// Analyze this repo and generate 3 feature ideas`
  <sub>Vision-stage or greenfield products.</sub>

- `// Identify tech debt in this file`
  <sub>Codebases with messy or fragile logic.</sub>

- `// Find duplicate logic across files`
  <sub>Sprawling repos lacking DRY practices.</sub>

- `// Cluster related functions and suggest refactors`
  <sub>Projects with lots of utils or helpers.</sub>

- `// Help me scope this issue so Jules can solve it`
  <sub>For working with Jules on real issues.</sub>

- `// Convert this function into a reusable plugin/module`
  <sub>Componentizing logic-heavy code.</sub>

- `// Refactor this Python function to be more amenable to parallel processing (e.g., using multiprocessing or threading)...`
  <sub>For optimizing performance in computationally intensive Python applications.</sub>

---

## Code Transformation & Modernization

The software development landscape is in constant flux. New languages, frameworks, and architectural patterns emerge, while existing codebases age, accumulating technical debt and potentially becoming vulnerable or inefficient. "Code Transformation & Modernization" is a critical category for "Awesome Jules Prompts" because it directly addresses the significant challenges developers face in keeping their software current, performant, and maintainable. Jules, as an advanced AI coding assistant, is uniquely positioned to help with these complex and often time-consuming tasks.

- `// Jules, I have a large Python 2 codebase in ./legacy_app. Help me migrate it to Python 3. Please identify key areas that need changes (like print statements, integer division, xrange, and library incompatibilities such as iteritems), and provide a plan or even attempt the initial conversion for a specific module, say utils.py.`
  <sub>Showcases: Language version migration, identification of breaking changes, and potentially automated code conversion.</sub>
- `// Jules, the file data_processor.java contains a monolithic processData() method that is over 500 lines long and difficult to maintain. Analyze this method and refactor it into smaller, more manageable private methods within the same class. Ensure that the overall public API of the DataProcessor class remains unchanged. Identify logical blocks of code that can be grouped together.`
  <sub>Showcases: Code refactoring for maintainability, breaking down complex functions, and preserving public interfaces.</sub>
- `// Our application uses an older version of the Stripe API (v2019-02-19) for payment processing. We need to update our PaymentService.js module to use the latest Stripe API version (v2023-10-16). Please identify all the deprecated API calls in our current implementation and update them according to the latest Stripe API documentation, paying close attention to changes in request/response structures and authentication methods. You can find the new API documentation at [link to hypothetical Stripe API docs].`
  <sub>Showcases: API version migration, handling changes in external dependencies, and potentially using external documentation.</sub>
- `// Jules, we're migrating our frontend from AngularJS to React. Take the following AngularJS component (./frontend/src/components/user-profile/user-profile.component.js and user-profile.template.html) and convert it into a functional React component using Hooks. Maintain the same core functionality and data bindings. Identify any AngularJS-specific services or filters used and suggest how they might be handled in a React context.`
  <sub>Showcases: Framework migration, component-based conversion, and handling framework-specific patterns.</sub>
- `// The SQL queries in our ./backend/src/report_generator.py module are constructed using string concatenation, making them vulnerable to SQL injection. Please refactor all database interaction methods in this file to use parameterized queries or an ORM like SQLAlchemy (if one is already in use or can be easily integrated). Explain the changes made and why they improve security.`
  <sub>Showcases: Security enhancement, refactoring for best practices, and preventing common vulnerabilities.</sub>

---

## Context

- `// Write a status update based on recent commits`
  <sub>Managerial and async communication.</sub>

- `// Summarize all changes in the last 7 days`
  <sub>Catching up after time off.</sub>



## Fun & Experimental

- `// Add a confetti animation when {a specific} action succeeds`
  <sub>Frontend web apps with user delight moments.</sub>

- `// Inject a developer joke when {a specific} build finishes`
  <sub>Personal projects or team tools.</sub>

- `// Build a mini CLI game that runs in the terminal`
  <sub>For learning or community fun.</sub>

- `// Add a dark mode Easter egg to this UI`
  <sub>Design-heavy frontend projects.</sub>

- `// Turn this tool into a GitHub App`
  <sub>Reusable, platform-integrated tools.</sub>

## Start from Scratch

- `// What's going to on in this repo?`
  <sub>Great for legacy repos or onboarding onto unfamiliar code.</sub>

- `// Initialize a new Express app with CORS enabled`
  <sub>Web backend projects using Node.js and Express.</sub>

- `// Set up a monorepo using Turborepo and PNPM`
  <sub>Multi-package JS/TS projects with shared dependencies.</sub>

- `// Bootstrap a Python project with Poetry and Pytest`
  <sub>Python repos aiming for clean dependency and test setup.</sub>

- `// Create a starter template for a Chrome extension`
  <sub>Browser extension development.</sub>

- `// I want to build a web scraper—start me off`
  <sub>Data scraping or automation tools using Python/Node.</sub>



## Contributing

Your contributions are welcome! Add new prompts, fix formatting, or suggest categories.

- 📄 [Contributing Guide](contributing.md)
- 🪄 Open a [Pull Request](https://github.com/YOUR_REPO/pulls)
