# Rest-API-Postman-Collection
# Rest API Automation with Postman, Newman, and Allure

This project automates the testing of REST APIs using **Postman**, **Newman**, and generates reports with **Allure**. It includes data-driven testing using external files.

## Features
- Postman collection for API automation.
- Environment-specific configurations using Postman environment files.
- Data-driven testing with JSON file.
- Command-line execution using Newman.
- Detailed test reports generated with Allure.

---

## Prerequisites
Ensure the following tools are installed on your system:
1. [Node.js](https://nodejs.org/) (includes npm)
2. [Newman](https://www.npmjs.com/package/newman)
3. [Allure CLI](https://github.com/allure-framework/allure2)

---

## Installation
### 1. Clone the Repository
```bash
git clone https://github.com/your-username/your-repository-name.git
cd your-repository-name
-Install Newman
-npm install -g newman
-Install Allure CLI
-npm install -g allure-commandline --save-dev

## Project Structure
.
- StudentAPI.postman_collection.json     # Postman collection
- Testenvironment.postman_environment.json  # Postman environment file
- Data.json                              # Test data for data-driven testing
- README.md                              # Project documentation

## Data driven testing
-newman run StudentAPI.postman_collection.json \
    -e Testenvironment.postman_environment.json \
    --iteration-data Data.json



