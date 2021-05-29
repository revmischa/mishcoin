## MishCoin

The official MISH ERC20 token for trading on ethereum mainnet.

A prototype created using the OpenZepplin `ERC20` interface and base `Contract`.

### Example

```solidity
// SPDX-License-Identifier: ABRMS
pragma solidity ^0.8.0;

import "https://github.com/OpenZeppelin/openzeppelin-contracts/blob/master/contracts/token/ERC20/ERC20.sol";

contract MishToken is ERC20 {
    constructor(uint256 initialSupply) ERC20("MishCoin", "MISH") {
        _mint(msg.sender, initialSupply);
    }
    
    function decimals() public view virtual override returns (uint8) {
        return 2;
    }
}
```
