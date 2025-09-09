# Selenium Page Object Model (POM) Example

This project is a demonstration of the Page Object Model (POM) design pattern for UI testing with Selenium and Python. It automates the login and logout process for the OrangeHRM demo website.

## Project Overview

The Selenium POM Example is a well-structured testing project that showcases how to use the Page Object Model to create maintainable and scalable UI tests. It separates the test logic from the UI interaction logic, making the tests easier to read and update.

This project is a great resource for anyone looking to learn about best practices in test automation with Selenium.

## Features

*   **Page Object Model (POM):** The project is structured using the POM pattern, with separate classes for the Login and Home pages.
*   **Automated login/logout:** The test script automates the process of logging in, verifying the home page, and then logging out.
*   **Uses `unittest`:** The tests are written using Python's built-in `unittest` framework.

## Technologies Used

*   **Language:** Python
*   **Testing Framework:** [Selenium](https://www.selenium.dev/)
*   **Test Runner:** [unittest](https://docs.python.org/3/library/unittest.html)

## Installation and Setup

To run these tests on your local machine, you'll need Python, pip, and Google Chrome.

1.  **Clone the repository:**
    ```bash
    git clone https://github.com/init050/POM.git
    cd POM
    ```

2.  **Create a virtual environment and activate it:**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use `venv\Scripts\activate`
    ```

3.  **Install the dependencies:**
    ```bash
    pip install selenium
    ```

4.  **Download ChromeDriver:**
    The script expects a `chromedriver.exe` file to be present. You'll need to download the version of ChromeDriver that corresponds to your version of Google Chrome.
    *   You can download ChromeDriver from the official website: [https://chromedriver.chromium.org/downloads](https://chromedriver.chromium.org/downloads)
    *   The script expects the driver to be in a `Driver` directory at the root of the project (i.e., `../Driver/chromedriver.exe`). You may need to create this directory and place the driver there, or update the path in `Login_Test_POM.py`.

## How to Use

Once you have everything set up, you can run the tests from the command line.

1.  **Navigate to the `POM` directory:**
    ```bash
    cd POM
    ```

2.  **Run the test script:**
    ```bash
    python Login_Test_POM.py
    ```

The script will launch a new Chrome browser window, navigate to the OrangeHRM demo site, and perform the login and logout actions.

## Future Improvements

*   **Cross-browser testing:** The tests could be configured to run on other browsers, like Firefox or Edge.
*   **Data-driven testing:** The login credentials are currently hardcoded. This could be improved by using a data-driven approach to test with multiple sets of user data.
*   **More comprehensive tests:** Add more test cases to cover different scenarios, like invalid logins or other features of the website.
*   **CI/CD integration:** Integrate the tests into a Continuous Integration/Continuous Deployment (CI/CD) pipeline to run automatically on every code change.
