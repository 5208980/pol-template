# Proof of Learn Template

This is a template and layout for Proof of Learn content. Use this as a base line to add content and resources to your POL then submit a PR to [TODO](#). Please note that the content and resource in this repository is AI generated and information and resource are done to provide placeholder to what a Proof of Learn template should be.

Notes:
- You can add custom folders to your resources, just make sure they do not beggin with a number, `{number}_`
    - See `you_can_add_custom_folder` or `assets` folders
- Resources can be a single topic or split into sub modules,
    - `01_deploy_your_first_token` has 6 submodules
    - `02_tokens_using_openzeppelin` is a single module
- quest and configurations for the resources, NFT metadata and requirements can be found in `quest.config.json`
    - See Docs (Coming soon) for `quest.config.json` schema

- If you resources wants to mint NFT for complete a modules or submodule, be sure to add it to quest.config.json
- This will ensure learners will deploy or transaction on specified chains for a given module
- To help validate, you can visit `/utility`
    - TODO: Add scripts to validate here.