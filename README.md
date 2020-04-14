# MyContract
# Variables, Data Types, Structs
pragma solidity ^0.6.0;

contract MyContract{
    //state variables
    string public myString = "Hello World";
    bytes32 public myBytes32 = "Hello World";
    int public myInt = 1;
    uint public myUint = 1;
    uint256 public myUint256 = 1;
    uint8 public myUint8 = 1;
    address public myAddress = 0xe5d6729C540E93178EF0A28F961edFdC01E63303;
    
    //structs
    struct MyStruct {
        uint myInt;
        string myString;
    }
    
    MyStruct public myStruct = MyStruct(1, "Hello World");
    
    // local variables
    function getValue() public pure returns(uint) {
        uint value = 1;
        return value;
    }
}
