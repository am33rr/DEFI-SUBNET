##  Deploying two contracts to Local Subnet

This project includes deploying the `ERC20` contract which includes all the basic ERC20 functions and the  `Vault` contract which includes depositing and withdrawing a specifeied number of shares to the local avalanche subnet created with our own configurations.

## Description

Firstly I created two files - 
- `ERC20.sol` pasted the ERC20 contract in this file
- `Vault.sol` pasted the IERC20 interface and the vault contract in this file.

Next, I set up my subnet and deployed it locally 

Then I interacted with the contract using the subnet i created 
## Subnet Configurations
**Type* - `Subnet-EVM`

**Name* - `mySubnett`

**Chain ID* - `3276`

**Symbol* - `AMR`

 
### Creating Subnet
 
1. In your Linux terminal , run the following command: `curl -sSfL https://raw.githubusercontent.com/ava-labs/avalanche-cli/main/scripts/install.sh | sh -s`
2. Run `export PATH=~/bin:$PATH`
3. Create subnet `avalanche subnet create mySubnett`
4. Deploy the subnet `avalanche subnet deploy mySubnett`

### Metamask Setup

Add Network -> Add network Manually ->

Name: mySubnett

RPC URL: http://127.0.0.1:9650/ext/bc/2UvKuRMHDvGVwPhLuvVv5UscE59rSgqYxciSKJDWd5AwLoPWPd/rpc

Chain ID: 3276

Symbol: AMR

`Save`

## Authors
 
Ameer S
 
email - [am33rrss@gmail.com]
 
## License
 
This project is licensed under the MIT License - see the LICENSE.md file for details
 
 
