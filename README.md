# Signup and Login Automation Project

This project automates the signup and login flow for a web application using Cypress with a Page Object Model (POM) design pattern. The tests ensure the functionality of user registration and subsequent login using dynamically generated user data.

## Project Structure

The project consists of the following key components:

1. **Page Objects**:
   - `SignupPage`: Contains methods for automating the signup process, including filling the form and navigating the required pages.
   - `LoginPage`: Contains methods for automating the login process.

2. **Test**:
   - A Cypress test suite to verify the signup and login functionality.

## Prerequisites

To run this project locally, ensure you have the following installed:

1. [Node.js](https://nodejs.org/) (version 14 or above)
2. [Cypress](https://www.cypress.io/) (version 12 or above)
3. A code editor like [VSCode](https://code.visualstudio.com/)

## Setup Instructions

Follow these steps to clone and run the project:

1. **Clone the Repository**:
   ```bash
   git clone <repository-link>
   cd <repository-name>
   ```

2. **Install Dependencies**:
   Install the required npm packages by running:
   ```bash
   npm install
   ```

3. **Run the Tests**:
   Execute the Cypress tests using:
   ```bash
   npx cypress open
   ```
   This will open the Cypress Test Runner. Select the test file to run.

## How the Project Works

1. **Signup Flow**:
   - Navigates to the signup/login page.
   - Clicks on the "Continue" button to access the signup form.
   - Fills the signup form with dynamically generated user data (unique email, name, etc.).
   - Submits the form and logs out after successful signup.

2. **Login Flow**:
   - Logs in using the same credentials used during signup.
   - Verifies successful login by checking for specific text or elements on the dashboard.

## Files Overview

1. **`SignupPage.js`**:
   - Methods: `navigate`, `generateRandomData`, `clickContinueButton`, `fillSignupForm`
   - Handles user registration by automating form interactions.

2. **`LoginPage.js`**:
   - Methods: `fillLoginForm`
   - Automates login using email and password.

3. **Test File**:
   - Contains the test case to verify the entire signup and login flow.

## Dependencies

The project uses the following npm packages:

- `cypress`: For end-to-end testing.
- `cypress-xpath`: To use XPath selectors in Cypress tests.

Install Cypress XPath with:
```bash
npm install -D cypress-xpath
```

## Notes for the Reviewer

- The test dynamically generates user data, ensuring each test run uses unique credentials.
- Adjust selectors and assertions as per the application's DOM and behavior.

## Contact

For any questions or support, please contact Kapil at kapil@adlerqa.in
