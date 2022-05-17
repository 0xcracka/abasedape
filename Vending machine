// SPDX-License-Identifier: MIT
pragma solidity 0.8.7;

contract VendingMachine{
     
     address public owner;
     mapping (address => uint) public dounutbalance;

     constructor () {
         owner = msg.sender;
         dounutbalance[addres(this)] = 100;

     }

    function getVendingMachineBalance() public view returns (unint){
        return dounutbalance[addres(this)];
    }

    function restock(uint amount) public {
        require(msg.sender = owner, "only the owner can restock this machine");
        dounutbalance[address(this)] += ammount;
    }

    function purchase (uint amount) public payable{
        require (msg.value >= amount * 2 ether, "you must pay at least 2 ether per donut");
        require (dounutbalance[address(this)]) >= amount, "not enough donuts in stock to fulfill request");
        dounutbalance[address(this)] -=amount;
        dounutbalance[msg.sender] += amount;

    }
}
