# Modifier variables to Your Solidity Contract

Setter functions allow us to update the state variables within our contract, enabling dynamic interactions with the blockchain.

## What is a Setter Function?

A setter function is a public function that allows us to modify the value of a state variable. Unlike getter functions, setter functions can alter the state of the contract. This is essential for contracts that need to update their data based on user inputs or other interactions.

Let's add a setter function to our `SimpleContract` to update the `value` variable.

## Step-by-Step Guide to Adding a Setter Function

### Step 1: Open Your Solidity Contract

Start by opening your Solidity code editor and loading your existing contract. Your contract should look something like this:

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract SimpleContract {
    string value;
    string name;
    
    // Existing getter function
    function getValue() public view returns (string memory) {
        return value;
    }
}
```

### Step 2: Add the Setter Function

Next, let's add a setter function to update the `value` variable. Update your contract to include the following function:

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract SimpleContract {
    string value;
    string name;
    
    // Existing getter function
    function getValue() public view returns (string memory) {
        return value;
    }
    
    // Add this setter function
    function setValue(string memory _value) public {
        value = _value;
    }
}
```

### What Just Happened?

By adding the setter function `setValue`, we've created a way to update the `value` variable from outside the contract. Let's break down the function to understand it better:

- **Function Keyword:** `function` is used to define a new function. Functions are blocks of code that can be called to perform specific tasks.

- **setValue:** This is the name of the function. Naming functions descriptively helps make your code more readable and understandable.

- **Parameters:** The function takes a single parameter, `_value`, of type `string memory`. The underscore prefix is a common convention to differentiate the parameter from the state variable with the same name.

- **Public:** This visibility modifier means the function can be called from outside the contract. It's essential for functions that need to be accessible by users or other contracts.

- **Function Body:** Inside the function, we assign the value of `_value` to the state variable `value`. This updates the state of the contract, changing the stored value on the blockchain.

### Understanding the State Mutability

Unlike getter functions, setter functions do not include the `view` keyword because they modify the state of the contract. When a setter function is called, it changes the contract's data, which is then permanently stored on the blockchain. This action incurs a gas fee, as writing to the blockchain is a resource-intensive operation.

Setter functions are crucial for contracts that need to adapt to changing conditions or inputs. They enable dynamic interactions, allowing users to update contract data based on their needs.

### Try It Yourself

I encourage you to experiment by adding setter functions for other variables. For example, add a setter function for the `name` variable. Here’s how you can do it:

```solidity
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract SimpleContract {
    string value;
    string name;
    
    // Getter for the 'value' variable
    function getValue() public view returns (string memory) {
        return value;
    }

    // Setter for the 'value' variable
    function setValue(string memory _value) public {
        value = _value;
    }

    // Getter for the 'name' variable
    function getName() public view returns (string memory) {
        return name;
    }

    // Setter for the 'name' variable
}
```

By adding the `setName` function, you've expanded the ways in which you can interact with your contract. The principles remain the same: the function is public and allows for updating a state variable based on user input. This pattern is fundamental in Solidity, ensuring that your contract can adapt and respond to user actions.

## Conclusion

Congratulations! You've successfully added setter functions to your Solidity contract. Setter functions are crucial for updating the state of your contract based on external inputs. This hands-on approach helps solidify your understanding of how to write data to the blockchain.

In the next section, we'll explore more advanced topics deploy and test our contract.