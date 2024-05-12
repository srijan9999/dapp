# DApp Sample using Hardhat on Windows with Visual Studio Code

This is a basic example of creating a decentralized application (DApp) using Hardhat on Windows with Visual Studio Code. 

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
  npm i create-react-app
  npx create-react-app yo
   ```
![image](https://github.com/srijan9999/dapp/assets/148010653/08487b2b-b523-478b-a5ad-e3e923bd7fa1)

3. **Change the directory by your app name (yo)**
   ```bash
   cd yo
   ```
4. **Install hardhat in the app folder**
   ```bash
   npm install hardhat
   ```
   ![image](https://github.com/srijan9999/dapp/assets/148010653/47b13a3c-062a-470c-b1f5-711448c8a1f2)

5. **Delete the readme file then run the entre twice to make the js file**
    ```bash
   npx hardhat
   ```
    ![image](https://github.com/srijan9999/dapp/assets/148010653/46ffab00-37e1-43e6-a460-a4f83b9df712)
6. **Open Cmd with administrator benefits and go to the vs code directory **
    ![image](https://github.com/srijan9999/dapp/assets/148010653/441e7161-6274-4ff8-aef5-746969a45406)


  

7. **Create a smart contract:**
   - In the `contracts` directory, create a new file named `SampleContract.sol`:

   ```solidity
  
   ```
  ![image](https://github.com/srijan9999/dapp/assets/148010653/f04ebd9f-9c7c-4271-88ff-069b88a65547)


8. **Write tests for the smart contract:**
   - In the `test` directory, create a new file named `sampleContract.test.js`:

   ```javascript
 
   ```
 ![image](https://github.com/srijan9999/dapp/assets/148010653/eda10fd8-b248-42eb-ac58-2ad54a15a103)


9. **Compile the contracts:**
   - Run the following command in the terminal:

   ```bash
   npx hardhat compile
   ```

10. **Write a frontend:**
   - Create an `index.html` file in the root directory.
      ```
     
       ```

   -![image](https://github.com/srijan9999/dapp/assets/148010653/f96aaccc-17db-4402-86f6-b3f076879da6)


11. **Deploy the contract locally:**
   - Run the following command in the terminal:

   ```bash
   npx hardhat node
   ```

12. **Interact with the frontend:**
   - Replace `"YOUR_CONTRACT_ADDRESS"` in the `index.html` file with the deployed contract address.
   - Open the `index.html` file in a web browser.
  

Now you have a simple DApp running locally! You can interact with the smart contract through the frontend.
 -![image](https://github.com/srijan9999/dapp/assets/148010653/c022946c-4a35-4e84-8cb7-6684c4c9f2fd)


