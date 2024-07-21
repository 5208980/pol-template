# Configuring MetaMask for Open Campus Codex

To interact with your deployed contract on a specific blockchain network, you'll need to configure MetaMask to connect to that network. In this section, we'll guide you through setting up MetaMask for the Open Campus Codex network.

### Step 5: Setting Up MetaMask

MetaMask is a popular browser extension wallet that allows you to interact with various blockchain networks. If you haven't installed MetaMask yet, you can download it from [MetaMask's official website](https://metamask.io/).

1. **Install MetaMask:** Follow the instructions on MetaMask's website to install the extension for your browser.
2. **Create an Account:** If you don't have an account, create a new one and securely store your seed phrase.

### Step 6: Adding the Open Campus Codex Network

To connect MetaMask to the Open Campus Codex network, follow these steps:

1. **Open MetaMask:** Click the MetaMask extension icon in your browser.
2. **Click the Network Dropdown:** At the top of the MetaMask window, click the network dropdown (it might say "Ethereum Mainnet" by default).
3. **Add a New Network:** Click "Add Network" to open the network configuration form.
4. **Enter Network Details:** Fill in the network details for Open Campus Codex. Here are the details you need (replace with actual details if available):

   - **Network Name:** Open Campus Codex
   - **New RPC URL:** `https://rpc.opencampuscodex.io`
   - **Chain ID:** `1234` (replace with the actual Chain ID)
   - **Currency Symbol:** `OCC` (replace with the actual symbol)
   - **Block Explorer URL:** `https://explorer.opencampuscodex.io` (optional)

5. **Save the Network:** Click "Save" to add the network to MetaMask.

Now, MetaMask is configured to use the Open Campus Codex network. You should see the network name at the top of the MetaMask window.

### Deploying and Interacting with Your Contract on Open Campus Codex

With MetaMask connected to the Open Campus Codex network, you can deploy and interact with your Solidity contract.

### Step 7: Deploying the Contract

2. **Compile Your Contract:** Ensure your contract is compiled using the correct compiler version as described earlier.
3. **Open the Deploy & Run Transactions Tab:** Navigate to the "Deploy & Run Transactions" tab on the left sidebar.
4. **Select the Environment:** Select "Injected Web3" from the "Environment" dropdown menu. use MetaMask for deploying the contract.
6. **Deploy the Contract:** Ensure that your contract is selected in the "Contract" dropdown menu. Click the "Deploy" button to deploy your contract to the Open Campus Codex network. MetaMask will prompt you to confirm the transaction.

### Step 8: Interacting with Your Contract

After deploying your contract, you can interact with it using the functions you defined.

1. **Find Your Deployed Contract:** Under "Deployed Contracts," expand your deployed contract to see its functions.
2. **Set a Value:** Call the `setValue` function by entering a string value (e.g., "Hello, Open Campus Codex!") and clicking the "transact" button. MetaMask will prompt you to confirm the transaction.
3. **Get the Value:** Call the `getValue` function by clicking the "call" button. You should see the string value you set earlier returned by this function.
4. **Set and Get Name:** Similarly, you can set and get the `name` state variable using the `setName` and `getName` functions.

### Conclusion

Congratulations! You've successfully configured MetaMask to use the Open Campus Codex network, deployed your Solidity contract, and interacted with it. This setup allows you to work on a specific blockchain network and test your smart contract in a real-world environment.
