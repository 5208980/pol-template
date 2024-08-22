# Proof of Learn (POL) 3 Template

Welcome to the **Proof of Learn 3 Template**! This template serves as your starting point for creating engaging and interactive learning content for the POL platform. All the content and resources you need can be found [in this GitHub repository](https://github.com/5208980/pol-template).

## Getting Started

All sections and guides in this template are created as Markdown files within the `/content` folder. This makes it easy to customize and expand upon the provided content as you build your own quests and learning resources.

The template comes with a pre-configured quest structure. The quest configuration file can be found [here](https://github.com/5208980/pol-template/blob/master/quest.config.json). Feel free to modify it to fit your specific needs.

### Explore the Template on POL

Once you’ve added your content, you can test it directly on POL. The platform's integrated IDE allows users to complete quests or alternatively use tools like Remix or Foundry.

### Structure of the Template

- **01_deploy_your_first_token**:  
  This is where users will begin their journey. It contains a step-by-step guide on deploying their first token, with two main quests:
  - **05_deploy**: This section walks users through deploying a smart contract. The goal is for users to create and deploy a contract, providing the transaction hash as proof. As a creator, you'll need to ensure your guide has clear instructions, including details about deploying to the correct blockchain and using the correct contract format.
  - **06_set**: Here, users will interact with their deployed contract by invoking a method or performing a transaction. The transaction hash will verify their success. Again, your guidance as a creator will be crucial to ensure users can correctly complete this task.
  
- **02_tokens_using_openzeppelin**:  
  This section covers deploying tokens using the popular `@openzeppelin` library. The quest in this section is more advanced, as it requires users to understand how to use external libraries to create and deploy smart contracts.
