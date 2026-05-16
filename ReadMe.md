# Dibimbing LMS Automation Testing

Automation testing project for **Dibimbing LMS** using:
- Selenium WebDriver
- TestNG
- Rest Assured
- GraphQL API Testing
- Extent Report
- Gradle Build Tool

This project covers both:
- **UI Automation Testing**
- **API Automation Testing**

---

# 📌 Tech Stack

| Technology | Description |
|---|---|
| Java | Programming Language |
| Selenium | UI Automation |
| TestNG | Test Framework |
| Rest Assured | API Automation |
| GraphQL | API Query & Mutation |
| Gradle | Dependency Management |
| Extent Report | Test Reporting |
| WebDriverManager | Browser Driver Management |
| Apache POI | Excel File Handling |

---

# 📂 Project Structure

```bash
project-root/
├── build.gradle
├── settings.gradle
├── testng.xml
├── reports/
├── src/
│   ├── main/
│   │   └── java/
│   │       ├── core/
│   │       │   ├── driver/
│   │       │   │   ├── DriverManager.java
│   │       │   │   ├── DriverFactory.java
│   │       │   │
│   │       │   ├── config/
│   │       │   │   ├── ConfigReader.java
│   │       │   │
│   │       │   ├── utils/
│   │       │   │   ├── TestUtils.java
│   │       │   │   ├── WaitUtils.java
│   │       │   │
│   │       │   ├── report/
│   │       │   │   ├── ExtentManager.java
│   │
│   │       ├── ui/
│   │       │   ├── pages/
│   │       │   │   ├── LoginPage.java
│   │       │   │
│   │       │   ├── base/
│   │       │       ├── BasePage.java
│   │
│   │       ├── api/
│   │           ├── client/
│   │           │   ├── ApiClient.java
│   │           ├── base/
│   │               ├── BaseApi.java
│
│   ├── test/
│       ├── java/
│       │   ├── ui/
│       │   │   ├── BaseTest.java
│       │   │   ├── LoginTest.java
│       │   │
│       │   ├── api/
│       │   │   ├── LoginApiTest.java
│       │   │
│       │   ├── listeners/
│       │       ├── TestListener.java
│       │
│       ├── resources/
│           ├── config.properties
│           ├── test-data/
│               ├── data.xlsx
```

---

# ✅ Features Covered

## UI Automation
- Login Testing
- Employee Management Testing
- Form Validation
- Navigation Testing

## API Automation
- Login API Testing
- Create Employee
- Update Employee
- Delete Employee
- GraphQL Request Validation
- Response Validation

---

# 🧪 Testing Approach

This project implements:
- Page Object Model (POM)
- Service Layer for API
- Reusable Base Test
- Centralized GraphQL Client
- Modular Test Design

---

# ⚙️ Prerequisites

Make sure the following are installed:

- Java JDK 17
- Gradle
- IntelliJ IDEA / VS Code
- Google Chrome

Check installation:

```bash
java -version
gradle -version
```

---

# 🚀 Installation

Clone repository:

```bash
git clone https://github.com/Raza-fahmi/dibimbing-lms-automation.git
```

Move to project directory:

```bash
cd dibimbing-lms-automation
```

Install dependencies:

```bash
gradle build
```

---

# ▶️ Run Automation Test

## Run All Test

```bash
gradle test
```

## Run TestNG Suite

```bash
gradle clean test
```

---

# 📄 Test Suite Configuration

Test suite configuration located at:

```bash
src/test/resources/suites/testng.xml
```

---

# 📊 Reporting

This project uses:
- Extent Report
- TestNG Report

After execution, reports can be found in:

```bash
test-output/
```

or

```bash
reports/
```

---

# 🔐 Environment Configuration

If environment variables are needed, configure using `.env` file.

Example:

```env
BASE_URL=https://your-environment-url.com
EMAIL=test@mail.com
PASSWORD=yourpassword
```

---

# 🧩 API Architecture

API automation uses:
- GraphQL Client
- Request Model
- Response Wrapper
- Service Layer Abstraction

Example tested mutation:
- createEmployee
- updateEmployee
- deleteEmployee

---

# 🖥️ UI Architecture

UI automation implements:
- BaseTest setup
- Reusable page object
- Centralized driver initialization
- Assertion validation using TestNG

---

# 📦 Dependencies

Main dependencies used:

```gradle
testImplementation 'org.testng:testng:7.10.2'
testImplementation 'org.seleniumhq.selenium:selenium-java:4.31.0'
testImplementation 'io.rest-assured:rest-assured:5.3.2'
implementation 'io.github.bonigarcia:webdrivermanager:5.9.1'
```

---

# 📌 Notes

- This project is intended for learning and automation practice.
- Supports UI and API end-to-end validation.
- Uses modular structure for easier maintenance and scalability.

---

# 👨‍💻 Author

Reza Fahmi Pahlevi
