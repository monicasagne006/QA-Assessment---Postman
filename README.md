# Postman Project 

  

## Table of Contents 

- [Introduction](#introduction) 

- [Features](#features) 

- [Requirements](#requirements) 

- [Installation](#installation) 

- [Usage](#usage) 

- [Collection Structure](#collection-structure) 

- [Environment Variables](#environment-variables) 

- [Running Tests](#running-tests) 

- [Acknowledgements](#acknowledgements) 

  

## Introduction 

This project contains a Postman collection for testing and interacting with the  API. It includes 2 endpoints and automated tests to ensure the API's functionality and performance. 

  

## Features 

- **Comprehensive Collection:** Includes 2 endpoints. 

- **Automated Tests:** Ensures the API's functionality and performance. 

- **Environment Variables:** Easily switch between different environments. 

- **Detailed Documentation:** Each request and test is well-documented. 

  

## Requirements 

- [Postman](https://www.postman.com/downloads/) installed on your machine. 

- [Newman](https://www.npmjs.com/package/newman) (optional, for running tests from the command line). 

  

## Installation 

1. **Clone the repository:** 

    ```sh 

    git clone https://github.com/your-username/your-repository.git 

    ``` 

2. **Open Postman:** 

   - Import the collection JSON file located in the `collections` directory. 

   - Import the environment JSON file located in the `environments` directory. 

  

## Usage 

1. **Select Environment:** 

   - Choose the appropriate environment from the dropdown in Postman. 

  

2. **Run Collection:** 

   - Click on the collection name. 

   - Click the "Run" button to execute all requests and tests in the collection. 

  

## Collection Structure 

- **Folders:** contains 2 folders (Basic Testing and Negative Testing). 

- **Requests:** Basic Testing  folder contains 3 requests and Negative Testing  folder contains 4 requests related to the functionality. 

- **Tests:** Automated tests for each request to validate responses. 

  

## Environment Variables 

The project uses environment variables to manage different configurations. The following variables are included: 

- `baseUrl`: The base URL for the API. 

- `apiKey`: The API key for authentication. 

- `userId`: A sample user ID for testing. 

  

To add or edit environment variables: 

1. Go to the "Environments" tab in Postman. 

2. Select the imported environment. 

3. Add or modify the necessary variables. 

  

## Running Tests 

### Using Postman 

1. Open Postman. 

2. Select the collection. 

3. Click the "Run" button. 

  

### Using Newman 

1. Install Newman: 

    npm install -g newman 

2. Run the collection:  

  newman run QA_Assessment_API_Testing.postman_collection.json -e QA.postman_environment.json -r htmlextra 

   

## Acknowledgements 

- [Postman](https://www.postman.com/) 

- [Newman](https://www.npmjs.com/package/newman) 

- Any other resources or libraries used in the project. 
