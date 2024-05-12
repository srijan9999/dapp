# DApp Sample using Hardhat on Windows with Visual Studio Code

This is a basic example of how to create a decentralized application (DApp) using Hardhat on Windows with Visual Studio Code. The DApp consists of a simple smart contract and a front end to interact with it.

## Prerequisites

- Node.js installed
- Visual Studio Code installed
- Basic knowledge of JavaScript and Solidity

## Steps

1. **Set up the project:**
   - Open Visual Studio Code.
   - Create a new folder for your project and open it in Visual Studio Code.
   - Open a terminal in Visual Studio Code.

2. **Initialize the project:**
   - Run the following commands in the terminal:

   ```bash
   npm init -y
   npm install --save-dev hardhat @nomiclabs/hardhat-waffle ethereum-waffle chai
   npx hardhat
   ```

   Follow the prompts to create a new Hardhat project.

3. **Create a smart contract:**
   - In the `contracts` directory, create a new file named `SampleContract.sol`:

   ```solidity
   // SPDX-License-Identifier: MIT
   pragma solidity ^0.8.0;

   contract SampleContract {
       string public greeting;

       constructor() {
           greeting = "Hello, World!";
       }

       function setGreeting(string memory _greeting) public {
           greeting = _greeting;
       }

       function getGreeting() public view returns (string memory) {
           return greeting;
       }
   }
   ```

4. **Write tests for the smart contract:**
   - In the `test` directory, create a new file named `sampleContract.test.js`:

   ```javascript
   const { expect } = require("chai");

   describe("SampleContract", function() {
       it("Should return the correct greeting", async function() {
           const SampleContract = await ethers.getContractFactory("SampleContract");
           const sampleContract = await SampleContract.deploy();
           await sampleContract.deployed();

           expect(await sampleContract.getGreeting()).to.equal("Hello, World!");

           // Change greeting
           await sampleContract.setGreeting("Hola, Mundo!");
           expect(await sampleContract.getGreeting()).to.equal("Hola, Mundo!");
       });
   });
   ```

5. **Compile the contracts:**
   - Run the following command in the terminal:

   ```bash
   npx hardhat compile
   ```

6. **Write a frontend:**
   - Create an `index.html` file in the root directory (see code snippet in previous message).

7. **Deploy the contract locally:**
   - Run the following command in the terminal:

   ```bash
   npx hardhat node
   ```

8. **Interact with the frontend:**
   - Replace `"YOUR_CONTRACT_ADDRESS"` in the `index.html` file with the deployed contract address.
   - Open the `index.html` file in a web browser.

Now you have a simple DApp running locally! You can interact with the smart contract through the frontend.


