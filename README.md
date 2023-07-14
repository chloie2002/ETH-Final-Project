# ETH-Final-Project

This Solidity program is a user input program in which the user may add and subtract tokens and monitor the balances.

## Description

This  is a simple contract written in Solidity, a programming language for building smart contracts for the Ethereum network. Future IT students may use this tool to create even more intricate and effective programming.

## Getting Started

### Executing program

Remix is an online Solidity IDE that you may use to run this application. To get started, go to https://remix.ethereum.org/.

When you are on the Remix website, click the "+" icon in the left sidebar to start a new file. Put a.sol extension to the file, such as HelloWorld.sol. The code below should be copied and pasted into the file:

### Installing


``` ethsolidity
contract MyToken {

    // public variables here
   string public tokenName = "CHLOIE";
   string public tokenAbbrv = "CHL";
   uint public totalSupply = 0;

    // mapping variable here
    mapping(address => uint) public balances;

    // mint function
    function mint (address _address, uint _value) public {
       totalSupply += _value;
       balances[_address] += _value;
    }

    // burn function
    function burn (address _address, uint _value) public {
       if (balances[_address] >= _value) {
          totalSupply -= _value;
          balances[_address] -= _value;
       }
    }
}

```

## Authors

Chloie Jane T. Cruz
8215697@ntc.edu.ph
