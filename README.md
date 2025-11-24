// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

import "@openzeppelin/contracts/token/ERC20/ERC20.sol";

contract USDTz is ERC20 {

    constructor() ERC20("Tether USD Bridged ZED20", "USDT.z") {
        uint256 supply = 27500000000 * 10 ** decimals();
        _mint(0xBb88A2C703eD961f4A478581E99fb34e35339121, supply);
    }
}
