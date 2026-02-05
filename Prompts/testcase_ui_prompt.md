Generate a Playwright Python test automation framework (POM) for the following test cases.

Conditions:
- Use Playwright and Python for browser automation, Pytest as the test framework and Page Object Model (POM) design pattern.
- Add requirements.txt file for dependencies. Add pytest.ini file for pytest configurations.
- Install the necessary dependencies using pip (e.g., playwright, pytest, playwright browsers).
- Use a configuration file to manage sensitive data like credentials.
- Add comments in the code for better readability and maintainability.
- The tests should be under root/tests folder, page objects under root/pages folder, and utilities under root/utils folder, data under root/data folder.
- The framework should have proper error handling and logging mechanisms. Logs and screenshots should be captured for errors of the test case, under logs and screenshots directories respectively.
- Use assertions to validate the expected results.
- Run the tests using pytest and ensure that they pass successfully. Re-run the tests, if failed.
- Report should be generated after test execution.


# Directory Structure:
root/
│── tests/
│   └── test_basic_auth.py
│── pages/
│   └── basic_auth_page.py
│── utils/
    logger.py
│── data/
│── logs/
│── screenshots/


Test Case:
Verify Basic Authentication Functionality
Description:
This test case verifies that the basic authentication functionality works correctly by accessing a protected resource with valid and invalid credentials.
Test Steps:
1. Navigate to the URL https://practice.expandtesting.com/basic-auth in mode headless=False.
2. Attempt to access the protected resource with valid credentials (username: "admin", password: "admin").
3. Verify that access is granted and the protected content is displayed.
4. Attempt to access the protected resource with invalid credentials (username: "invalid", password: "invalid").
5. Verify that access is denied and an appropriate error message is displayed.
Expected Result:
- Access granted with valid credentials and the protected content is displayed.
- Access denied with invalid credentials and an appropriate error message is displayed.
