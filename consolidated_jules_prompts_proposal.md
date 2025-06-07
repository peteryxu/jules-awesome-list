Hello!

This message outlines three feature ideas to enhance the "Awesome Jules Prompts" list, aiming to expand its utility and comprehensiveness for developers.

Here are the proposals:

### 1. New Category: Code Transformation & Modernization

*   **Rationale:** This category addresses the critical need for updating and refactoring existing codebases. Jules can help accelerate legacy code migration (e.g., Python 2 to 3), automate complex refactoring for better maintainability, streamline API updates, enhance performance, and reduce developer toil associated with modernization efforts.
*   **Key Example Prompts:**
    *   "Jules, I have a large Python 2 codebase in `./legacy_app`. Help me migrate it to Python 3, identifying key changes like `print` statements, integer division, and library incompatibilities for a module like `utils.py`."
    *   "Jules, refactor the monolithic `processData()` method in `data_processor.java` (over 500 lines) into smaller, manageable private methods, ensuring the public API remains unchanged."
    *   "Our `PaymentService.js` uses an old Stripe API version. Update it to the latest version, identifying deprecated calls and changes in request/response structures based on the new API docs."

### 2. New Category: Security & Compliance

*   **Rationale:** Security and compliance are paramount in modern software development. This category will showcase Jules' ability to assist in early vulnerability detection (e.g., OWASP Top 10), promote secure coding practices, automate repetitive security tasks (like generating CSP headers), help with dependency vulnerability awareness, and offer guidance on aligning code with compliance principles (e.g., GDPR, HIPAA), acting as a "security champion" assistant.
*   **Key Example Prompts:**
    *   "Review `UserInputHandler.java` for XSS and SQL Injection vulnerabilities. Explain the risks and suggest code changes using prepared statements and proper output encoding."
    *   "Analyze `package.json` in `./my-app/` for dependency vulnerabilities. List CVEs, severity, and suggest minimum patched versions or generate an `npm audit fix` command."
    *   "Generate Python Flask code for robust input validation (username, email, password) in `./auth/routes.py` and explain how it prevents common security issues."

### 3. Enhancement to "Testing" Category: New Subcategories

*   **Proposal:** Enhance the existing "Testing" category by adding two new subcategories: "Test Data Generation" and "Test Strategy & Planning."
*   **Rationale for "Test Data Generation":** Address the challenge of creating diverse and realistic test data. Jules can automate data creation in various formats (JSON, CSV, SQL), cover edge cases, help anonymize sensitive data, and generate data for specific scenarios.
    *   **Key Example Prompts (Test Data Generation):**
        *   "Generate 10 valid and 3 invalid JSON user profiles with fields like `userId`, `username`, `email`, `dateOfBirth` (user >= 18), `isActive`."
        *   "Create a sample CSV with 20 realistic product entries (`product_id`, `name`, `category`, `price`, `stock_quantity`), including some with zero stock."
*   **Rationale for "Test Strategy & Planning":** Assist with higher-level testing aspects. Jules can help brainstorm test scenarios, identify appropriate test types, outline basic test plans, and suggest test case prioritization.
    *   **Key Example Prompts (Test Strategy & Planning):**
        *   "For a new 'Product Wishlist' e-commerce feature, brainstorm key test scenarios (functional, usability, negative tests)."
        *   "What test types (functional, security, performance) should be prioritized for a new social media REST API (endpoints: register, login, post, feed) and why?"

---

These proposed additions aim to significantly broaden the scope of "Awesome Jules Prompts," providing even more value to developers by covering crucial areas of the software development lifecycle.
