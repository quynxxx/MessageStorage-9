# MessageStorage-9
MessageStorage.sol
// SPDX-License-Identifier: MIT
pragma solidity ^0.8.20;

contract MessageStorage {
    string[] public messages;

    function addMessage(string memory _message) public {
        messages.push(_message);
    }

    function getAllMessages() public view returns (string[] memory) {
        return messages;
    }

    function getMessage(uint256 index) public view returns (string memory) {
        return messages[index];
    }
}
