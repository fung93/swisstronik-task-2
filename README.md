# SWISSTRONIK Technical Task 2

Steps to mint 100 ERC-20 Tokens

1. Clone repository
```shell
https://github.com/fung93/swisstronik-task-2.git
cd swisstronik-task-2
```
2. Make erc20.sh script executable
```shell
chmod +x erc20.sh
```
3. Run the script
```shell
./erc20.sh
```
4. Import Private Key
```shell
PRIVATE_KEY="your private key"
```
5. Create smart contract
```shell
// SPDX-License-Identifier: UNLICENSED
pragma solidity ^0.8.9;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";

contract TestToken is ERC20 {
    constructor()ERC20("FUNG","FNG"){} 

    function mint100tokens() public {
        _mint(msg.sender,100*10**18);
    }

    function burn100tokens() public{
        _burn(msg.sender,100*10**18);
    }
    
}
```
6. Mint token
7. Transfer token
8. Finished
   - Copy the address and paste the address to testnet dashboard
   - Copy the transaction link to testnet dashboard
   - Push this project to your github and paste the repository link to testnet dashboard

