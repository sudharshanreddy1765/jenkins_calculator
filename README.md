# Jenkins Calculator

A Java-based calculator application configured with an automated Continuous Integration (CI) pipeline using **Jenkins**, **Maven**, and **GitHub Webhooks**.

---

## 🚀 Features

- **Arithmetic Operations**: Addition, Subtraction, Multiplication, and Division.
- **Unit Testing**: Complete test coverage using JUnit.
- **Automated CI/CD**: Declarative `Jenkinsfile` for automated build and execution of unit tests on every code push.
- **Webhook Integration**: Real-time pipeline triggers using GitHub Webhooks and ngrok.

---

## 🛠️ Tech Stack

- **Language**: Java 17+
- **Build Tool**: Apache Maven
- **Testing Framework**: JUnit
- **CI/CD Automation**: Jenkins Pipeline
- **Tunneling / Webhook**: ngrok

---

## 📋 CI/CD Pipeline Stages

1. **Checkout SCM**: Pulls the latest code from the `master` branch.
2. **Tool Install**: Automatically configures `Maven 3.9`.
3. **Build Stage**: Executes `mvn clean compile` to compile the Java source files.
4. **Test Stage**: Executes `mvn test` to run the JUnit test suite.

---

## 💻 Running Locally

### Prerequisites

- Java Development Kit (JDK 17 or higher)
- Apache Maven
- Git

### Build & Run Tests

```bash
# Clone the
git clone [https://github.com/sudharshanreddy1765/jenkins_calculator.git](https://github.com/sudharshanreddy1765/jenkins_calculator.git)

# Navigate into the project directory
cd jenkins_calculator

# Run unit tests
mvn clean test
