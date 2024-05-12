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

   ![image](https://github.com/srijan9999/dapp/assets/148010653/7606eb9a-f57e-43aa-8773-8a565a390353)


4. **Create a smart contract:**
   - In the `contracts` directory, create a new file named `SampleContract.sol`:

   ```solidity
  
   ```
  ![image](https://github.com/srijan9999/dapp/assets/148010653/f04ebd9f-9c7c-4271-88ff-069b88a65547)


5. **Write tests for the smart contract:**
   - In the `test` directory, create a new file named `sampleContract.test.js`:

   ```javascript
 
   ```
 ![image](https://github.com/srijan9999/dapp/assets/148010653/eda10fd8-b248-42eb-ac58-2ad54a15a103)


6. **Compile the contracts:**
   - Run the following command in the terminal:

   ```bash
   npx hardhat compile
   ```

7. **Write a frontend:**
   - Create an `index.html` file in the root directory.
      ```
     
       ```

   - ![image](https://github.com/srijan9999/dapp/assets/148010653/f96aaccc-17db-4402-86f6-b3f076879da6)


8. **Deploy the contract locally:**
   - Run the following command in the terminal:

   ```bash
   npx hardhat node
   ```

9. **Interact with the frontend:**
   - Replace `"YOUR_CONTRACT_ADDRESS"` in the `index.html` file with the deployed contract address.
   - Open the `index.html` file in a web browser.

Now you have a simple DApp running locally! You can interact with the smart contract through the frontend.


