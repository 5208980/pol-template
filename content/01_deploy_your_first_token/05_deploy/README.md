# Deploy a Smart Contract

This section provides a template that allows creators to configure a deployment quest using the [quest.config.json template](https://github.com/5208980/pol-template/blob/master/quest.config.json). With this template, users can submit deployment transactions on specific chains.

In the configuration example below, we demonstrate deploying a contract on the Open Campus Codex chain. The contract used in this example is a simple Solidity contract:

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract SimpleContract {
    string public name;

    function set(string memory _name) public {
        name = _name;
    }
}
```

This section could include similar contract examples or allow users to customize their own deployments based on the setup provided.
Here's a clearer and more detailed continuation of your instructions:
## Setting Up MetaMask

MetaMask is a popular browser extension wallet that allows you to interact with various blockchain networks. If you haven't installed MetaMask yet, you can download it from [MetaMask's official website](https://metamask.io/). Once installed, you'll be able to manage your accounts, store your private keys securely, and interact with decentralized applications (dApps).

## Adding the Open Campus Codex Network

To deploy your contract to the Open Campus Codex network, you'll need to add this custom network to MetaMask. Follow these steps:

1. Open MetaMask and click on the network dropdown at the top.
2. Select "Add Network" and fill in the following details:

   - **Network Name:** Open Campus Codex  
   - **New RPC URL:** `https://open-campus-codex-sepolia.drpc.org`  
   - **Chain ID:** `656476`  
   - **Currency Symbol:** `EDU`  
   - **Block Explorer URL:** `https://opencampus-codex.blockscout.com/`

3. Click "Save."

Once saved, MetaMask is now configured to use the Open Campus Codex network. You should see the network name at the top of the MetaMask window.

## Deploying and Interacting with Your Contract on Open Campus Codex

With MetaMask connected to the Open Campus Codex network, you're ready to deploy and interact with your Solidity contract.

### Step 1: Compile the Contract

- Set your Solidity compiler version to **0.8.23**.
- Compile the `SimpleContract` from the earlier example.

### Step 2: Deploy the Contract

- After compilation, deploy the `SimpleContract` to the Open Campus Codex network. MetaMask will prompt you to approve the transaction for deployment.

Once the transaction is confirmed, your contract is successfully deployed!

### Step 3: Interact with the Contract

- You can now interact with your deployed contract using MetaMask. This includes calling the `set` function to change the `name` variable or querying the contract to view its current state.

Congratulations! You've successfully configured MetaMask for the Open Campus Codex network, deployed your Solidity contract, and interacted with it. 

### Final Step: Submit the Deployment to POL

To complete this quest, submit your deployed contract transaction to the Proof of Learn (POL) platform. This confirms that you've successfully deployed the contract.

## Next Steps: Interacting with Your Contract

In the next section, we'll guide you through interacting with your deployed contract, including how to change the variable `name` and update the contract state using its functions.