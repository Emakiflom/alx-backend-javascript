# 0x04. Typescript

## Resources
### Read or watch:
- [TypeScript in 5 minutes](https://www.typescriptlang.org/docs/handbook/typescript-in-5-minutes.html)
- [TypeScript documentation](https://www.typescriptlang.org/docs/)

### Learning Objectives
At the end of this project, you are expected to be able to explain to anyone, without the help of Google:
- Basic types in TypeScript
- Interfaces, Classes, and functions
- How to work with the DOM and TypeScript
- Generic types
- How to use namespaces
- How to merge declarations
- How to use an ambient Namespace to import an external library
- Basic nominal typing with TypeScript

### Requirements
- Allowed editors: `vi`, `vim`, `emacs`, `Visual Studio Code`
- All your files should end with a new line
- All your files will be transpiled on Ubuntu 18.04
- Your TS scripts will be checked with `jest` (version 24.9.*)
- A `README.md` file, at the root of the folder of the project, is mandatory
- Your code should use the `ts` extension when possible
- The TypeScript compiler should not show any warning or error when compiling your code

### Configuration Files
Please use these files for the following tasks:

#### package.json
```json
{
  "name": "typescript_project",
  "version": "1.0.0",
  "description": "TypeScript project",
  "main": "index.js",
  "scripts": {
    "build": "webpack",
    "test": "jest"
  },
  "author": "",
  "license": "ISC",
  "dependencies": {
    "typescript": "^3.8.3"
  },
  "devDependencies": {
    "jest": "^24.9.0",
    "ts-jest": "^24.0.2",
    "webpack": "^4.42.0",
    "webpack-cli": "^3.3.11"
  }
}

