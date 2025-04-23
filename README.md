OrangeHRM Automation Framework

This project is a complete, end-to-end test automation solution for OrangeHRM. It uses a combination of Java, Selenium WebDriver, TestNG, and Excel for managing test data.

Tech Stack

Here are the main technologies used:

Java
Selenium WebDriver
TestNG
Maven
Page Object Model (POM)
Excel (using Apache POI)
Git & GitHub


src/main/java/pages: This is where I keep all my page classes. I used the Page Object Model (POM) design pattern to make the code reusable and easier to manage. For example, if I was testing a login page, I’d have a LoginPage.java class here with methods like enterUsername() and clickLoginButton() to interact with the page elements.

src/test/java/tests: This folder holds all my TestNG test classes. I wrote my actual test cases here, like LoginTests.java or DashboardTests.java. These classes use the page objects from the pages folder to run the tests, keeping everything modular and clean.

src/main/java/utils: I put all my utility classes in this folder. For example, I have a WebDriverSetup.java class to handle browser setup and teardown, and an ExcelReader.java class to read test data from Excel files. These utilities help keep my test code DRY (Don’t Repeat Yourself) and make it easier to manage things like WebDriver instances or external data sources.

testdata.xlsx: This is the Excel file I use to store test data. For instance, it might have columns like Username, Password, and ExpectedResult for login tests. My ExcelReader utility class reads this data and feeds it into the test cases, so I can easily update test data without touching the code.

I found this structure really helpful because it kept everything organized and made it easy to scale the framework as the project grew. For example, when I worked on the automation framework for Caratred Technologies (March 2023 - Nov 2024), I used this setup to build end-to-end tests with Selenium, Java, TestNG, Cucumber, and Jenkins, and it saved me a ton of time when adding new features or debugging issues

