# Luma Shopping Website Testing - SDET Project

This repository contains the test scripts, test cases, and reports for testing the **Luma Shopping Website**. This project was carried out as part of a **Software Development Engineer in Test (SDET)** project during the construct week. The main focus was on both **manual** and **automated testing** using **Cypress**. It includes various test scenarios such as **login**, **create account**, **product search**, **cart process check**, and the identification of different **bugs** and **issues**.

## Project Overview

The **Luma Shopping Website** is an e-commerce platform that allows users to browse products, create accounts, log in, add products to the cart, and make purchases. The website also features user authentication, product search, and various other functionalities crucial for a seamless online shopping experience.

### Team Members
- **Puja Kumari** – Lead Tester
- **Yogesh Kumar** – Automation Tester

---

## Table of Contents
1. [Testing Scenarios](#testing-scenarios)
2. [Manual Testing](#manual-testing)
3. [Automated Testing with Cypress](#automated-testing-with-cypress)
4. [Bug Reports](#bug-reports)
5. [Test Cases](#test-cases)
6. [Mind Map](#mind-map)
7. [Collaboration and Workflow](#collaboration-and-workflow)
8. [Project Setup](#project-setup)

---

## Testing Scenarios

The primary testing scenarios include:

1. **Login**: Test the ability for users to log in with valid and invalid credentials.
2. **Create Account**: Verify the account creation functionality, including form validation and successful registration.
3. **Product Search**: Validate that users can search for products and view correct results.
4. **Cart Process Check**: Ensure that products can be added to the cart, the cart displays the correct products, and the checkout process works.
5. **Checkout Process**: Simulate a successful purchase and verify the successful completion of the order.

---

## Manual Testing

### Test Cases

- **Test Case 1: Login with valid credentials**
  - **Pre-condition**: User must have a registered account.
  - **Steps**:
    1. Navigate to the login page.
    2. Enter valid username and password.
    3. Click on "Login".
  - **Expected Output**: User should be redirected to the homepage.

- **Test Case 2: Create a new account**
  - **Pre-condition**: User does not have an existing account.
  - **Steps**:
    1. Navigate to the registration page.
    2. Fill in all required fields.
    3. Submit the form.
  - **Expected Output**: User should be successfully registered and logged in.

- **Test Case 3: Product Search**
  - **Pre-condition**: The website contains products.
  - **Steps**:
    1. Enter a product name in the search bar.
    2. Click on the search button.
  - **Expected Output**: Product(s) related to the search term should be displayed.

- **Test Case 4: Add Product to Cart**
  - **Pre-condition**: Product is available on the website.
  - **Steps**:
    1. Browse through the product catalog.
    2. Click on a product and add it to the cart.
  - **Expected Output**: Product is successfully added to the cart.

- **Test Case 5: Checkout Process**
  - **Pre-condition**: Product is in the cart.
  - **Steps**:
    1. Click on the cart icon.
    2. Proceed to checkout.
    3. Enter shipping and payment details.
    4. Submit the order.
  - **Expected Output**: The order is successfully processed and confirmed.

---

## Automated Testing with Cypress

### Automated Test Cases
Automated tests were created using **Cypress** to speed up regression testing and ensure consistent test execution. The following are the automated test cases:

1. **Login Test**: Automated script to verify user login functionality with valid and invalid credentials.
2. **Account Creation Test**: Automated test for user account registration and validation of form fields.
3. **Product Search Test**: Automated search functionality test to ensure the correct display of product results.
4. **Add to Cart Test**: Automation for adding products to the cart and verifying the cart.
5. **Checkout Test**: End-to-end automated test to simulate a full checkout process.

### Cypress Installation
To run the automated tests:

1. Clone this repository.
2. Navigate to the project directory in your terminal.
3. Install dependencies:
    ```bash
    npm install
    ```
4. Open Cypress:
    ```bash
    npx cypress open
    ```
5. Select the test to run in the Cypress interface.

---

## Bug Reports

During testing, the following bugs were identified:

1. **Bug #1: Login Failure with Correct Credentials**
   - **Steps to Reproduce**: Enter valid credentials and click on Login.
   - **Expected Behavior**: The user should be logged in.
   - **Actual Behavior**: The user was not redirected to the homepage.
   - **Severity**: High
   - **Resolution**: The issue was traced to a session handling bug and was fixed by the backend team.

2. **Bug #2: Missing Product Search Results**
   - **Steps to Reproduce**: Search for a product (e.g., "T-shirt").
   - **Expected Behavior**: Product results should be displayed.
   - **Actual Behavior**: No results were displayed even though products existed.
   - **Severity**: Medium
   - **Resolution**: Fixed by adjusting the search algorithm.

---

## Test Cases

A comprehensive list of all manual and automated test cases is documented in the **`test-cases`** folder. Each test case includes the steps to reproduce, expected outcomes, and severity.

---

## Mind Map

A visual representation of the testing process and test case coverage is included in the **`mind-map.png`** file. This mind map was used to plan the test scenarios, track testing progress, and ensure that all functionalities were covered.

---

## Collaboration and Workflow

### Collaboration Between Team Members
- **Puja Kumari** focused on manual testing, identifying critical issues, and preparing bug reports.
- **Yogesh Kumar** focused on writing and executing automated tests using **Cypress** to speed up the regression cycle and validate critical paths.

We used **Git** for version control and **Jira** for task management and issue tracking. Regular communication was maintained through **Slack** to ensure smooth collaboration.

### Conflict Resolution
In one instance, there was a disagreement between team members regarding the priority of manual vs. automated tests. After discussion, we agreed to focus on automating high-impact test cases while manually testing edge cases to ensure both speed and thoroughness.

---

## Project Setup

To set up this project locally:

1. **Clone the repository**:
    ```bash
    git clone https://github.com/pujakumari/LumaProject.git
    ```
2. **Install dependencies**:
    ```bash
    npm install
    ```
3. **Run Cypress tests**:
    ```bash
    npx cypress open
    ```

---

## Conclusion

This project demonstrates the testing efforts of the **Luma Shopping Website**, including both manual and automated testing approaches. The collaboration between the manual testing and automation teams allowed us to thoroughly test the application, identify bugs, and ensure its functionality before release.

For any additional information or assistance, feel free to contact us!

---

**Puja Kumari**  
**SDET Intern**  
**puja291196m@gmail.com**
