# TodoSimple.sol
Remix - Deploy Contract On Base Network TodoSimple.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract TodoSimple {
    string[] public todos;

    function add(string memory _task) public {
        todos.push(_task);
    }

    function getCount() public view returns (uint) {
        return todos.length;
    }
}
