# ETH-AVAL INTERMEDIATE 3

AnyToken Contract

License This contract is using the MIT License.

Prerequisites Solidity ^0.8.9

Contract Details: The contract imports three contracts from the OpenZeppelin library:

The code defines a custom token contract called "AnyToken" that inherits functionality from three contracts in the OpenZeppelin library: ERC20, ERC20Burnable, and Ownable.

The ERC20 contract is a standard implementation of the ERC20 token standard, which provides basic functionality for a fungible token. It includes functions such as transferring tokens, approving token transfers, and checking token balances.

The ERC20Burnable contract extends the ERC20 contract and adds the ability to burn (destroy) tokens. This allows token holders to permanently remove tokens from circulation.

The Ownable contract provides a basic access control mechanism, allowing only the contract owner to execute certain functions. It includes a modifier called "onlyOwner" that can be applied to functions to restrict their execution to the contract owner.

The CustomToken contract itself is defined and inherits from ERC20, ERC20Burnable, and Ownable. It does not introduce any additional functionality beyond what is inherited from these contracts.

The constructor function is defined without any parameters and is executed once when the contract is deployed. Within the constructor, the ERC20 constructor is called with the name "MyToken" and symbol "MyTk" to initialize the token with these values.

The mint function is a public function that can only be called by the contract owner (as defined by the Ownable contract). It takes two parameters: "to" (the address to which the tokens will be minted) and "amount" (the number of tokens to mint). Inside the function, the _mint function from the ERC20 contract is called to create and assign the specified amount of tokens to the given address.
https://www.loom.com/share/fcaa6a6ffe4c4b63a65268f680ba5883
