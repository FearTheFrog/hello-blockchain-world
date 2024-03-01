# Installation Commands for Truffle, Node.js, and npm

Before starting with the Hello World blockchain program, ensure you have Node.js, npm, and the Truffle framework installed. Here are the commands to install these tools:

## Install Node.js and npm

Visit the official Node.js website to download and install Node.js. npm is included with Node.js installation. https://nodejs.org/en/download

## Install Truffle

Once Node.js and npm are installed, use the following npm command to install Truffle globally:

```bash
npm install -g truffle
```

# Hello World Blockchain Program in Solidity

## Create a New Project

```bash
truffle init hello-world
cd hello-world
```

## Write the Smart Contract

```solidity
pragma solidity ^0.8.0;

contract HelloWorld {
    string public message = "Hello World!";
}
```

## Compile the Smart Contract

```bash
truffle compile
```

## Deploy the Smart Contract

```bash
truffle migrate
```

## Interact with the Smart Contract

```bash
truffle console
```

## Access the "Hello World" Message

```javascript
let instance = await HelloWorld.deployed()

let message = await instance.message()

console.log(message)  // Output: "Hello World!"
```
