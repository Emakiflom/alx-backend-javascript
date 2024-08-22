# 0x06. Unittests in JS

## Overview

This project focuses on writing unit tests and integration tests for Node.js applications using popular testing frameworks and libraries like Mocha, Chai, and Sinon. The goal is to ensure that you understand how to create robust test suites, manage asynchronous code in tests, and simulate external dependencies using spies and stubs.

## Learning Objectives

By the end of this project, you should be able to:

- Use Mocha to write comprehensive test suites.
- Employ different assertion libraries like Node's built-in assert module and Chai.
- Organize and present long test suites effectively.
- Utilize spies and stubs to mock behavior and control test environments.
- Understand and implement hooks in test suites.
- Perform unit testing with asynchronous functions.
- Write integration tests for small Node.js servers.

## Project Requirements

- **Environment:** All code will be executed on Ubuntu 18.04 LTS using Node.js version 12.x.x.
- **Editors:** vi, vim, emacs, Visual Studio Code.
- **File Extensions:** All files should use the `.js` extension.
- **README:** A `README.md` file at the root of the project is mandatory.
- **Newline:** All files should end with a new line.
- **Testing:** When running tests with `npm run test *.test.js`, all tests should pass without any warnings or errors.

## Setup

1. Clone the repository.
2. Install the necessary dependencies:
    ```bash
    npm install
    ```
3. Run the test suite using:
    ```bash
    npm run test *.test.js
    ```

## Key Concepts

### 1. Mocha

Mocha is a feature-rich JavaScript test framework running on Node.js, making asynchronous testing simple and fun. Mocha tests run serially, allowing for flexible and accurate reporting while mapping uncaught exceptions to the correct test cases.

### 2. Chai

Chai is an assertion library commonly used with Mocha. It provides a variety of assertion styles, including BDD-style `expect` and `should`, as well as TDD-style `assert`.

### 3. Sinon

Sinon is a standalone test spy, stub, and mock library for JavaScript. It works with any testing framework and is particularly useful for simulating behaviors in functions or methods, especially when dealing with external dependencies.

### 4. Spies and Stubs

- **Spies:** Monitor and track the behavior of functions during tests, checking how many times a function was called and with what arguments.
- **Stubs:** Replace a function with a specific implementation in a controlled way during testing, ideal for simulating external dependencies.

### 5. Hooks

Mocha provides hooks like `before`, `after`, `beforeEach`, and `afterEach` to manage setup and teardown in your test suites, ensuring that each test runs in a consistent environment.

### 6. Unit Testing with Async Functions

Testing asynchronous code requires special attention, using patterns like Promises, async/await, and callbacks correctly to ensure tests run predictably.

### 7. Integration Testing

Integration tests assess how different parts of your application work together. In this project, you will learn to test routes in a small Node.js server to ensure they behave as expected when accessed via HTTP requests.

## Example Test

Here is an example of a basic Mocha test with Chai assertions:

```javascript
const { expect } = require('chai');

describe('Sample Test', () => {
    it('should return true', () => {
        expect(true).to.equal(true);
    });
});

