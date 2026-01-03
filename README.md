OpenCart Automation Testing Project

This project demonstrates basic end-to-end automation testing of the OpenCart demo e-commerce website using Selenium WebDriver, Java, and TestNG.
It covers login functionality and product search validation with a structured test suite.

📌 Project Overview

Application Under Test: https://demo.opencart.com

Automation Tool: Selenium WebDriver

Language: Java

Test Framework: TestNG

Browser: Google Chrome

Design Pattern: Base Test setup with reusable WebDriver configuration

📂 Project Structure
├── BaseTest.java        // WebDriver & browser setup
├── LoginTest.java       // Automated login test
├── SearchTest.java      // Automated product search test
├── testng.xml           // Test suite configuration
└── README.md

⚙️ Prerequisites

Before running the project, ensure you have:

Java JDK (8 or above)

Google Chrome browser

ChromeDriver (matching your Chrome version)

Maven or IDE with TestNG support (IntelliJ / Eclipse)

TestNG library added to the project

🔧 Setup Instructions

Clone or download the project

Update ChromeDriver path in BaseTest.java:

System.setProperty("webdriver.chrome.driver", "path/to/chromedriver");


Ensure required dependencies (Selenium & TestNG) are added

Open the project in your IDE

🧪 Test Scenarios Covered
✅ Login Test

Navigate to My Account → Login

Enter valid email and password

Verify successful login using dashboard element

🔍 Product Search Test

Enter a product name in the search box

Perform search

Validate search results page

▶️ How to Run the Tests
Option 1: Using TestNG XML

Right-click on testng.xml

Select Run

Option 2: Using IDE

Right-click on individual test classes

Run as TestNG Test

📑 Test Suite Configuration

The testng.xml runs both tests sequentially:

<suite name="Ecommerce Test Suite">
    <test name="Login and Search Tests">
        <classes>
            <class name="LoginTest"/>
            <class name="SearchTest"/>
        </classes>
    </test>
</suite>

✅ Expected Results

Browser launches successfully

Login test passes for valid credentials

Product search displays correct results

Browser closes after test execution

🚀 Key Highlights

Reusable WebDriver setup

Clean TestNG structure

Assertion-based validation

Beginner-friendly Selenium automation project

Suitable for QA / Automation Intern roles

🧩 Future Enhancements

Page Object Model (POM)

Data-driven testing

Explicit waits

Test reports (Extent / Allure)

CI integration (Jenkins / GitHub Actions)

👩‍💻 Author

Anusha Sharma
B.Tech CSE | QA & Automation Enthusiast
