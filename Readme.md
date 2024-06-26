# Project Title  
Create a Token.

## Description  
This Solidity contract, MyToken, defines a simple token with public variables for the token name, abbreviation, and total supply. It includes functions to mint (create) new tokens and assign them to an address, and to burn (destroy) tokens from an address, while maintaining a mapping of token balances for each address.

# Getting Started

## Installing  
To run this program, you can use Remix, an online Solidity IDE. To get started, go to the Remix website at https://remix.ethereum.org/.

Once you are on the Remix website, create a new file by clicking on the "+" icon in the left-hand sidebar. Save the file with a .sol extension (e.g., HelloWorld.sol). Copy and paste the following code into the file:

```javascriptf
pragma solidity >=0.6.12 <0.9.0;

contract MyToken {

    // public variables here
    string public token  ="Muskan sharma";
      uint public  totsupply=0;
    string public tokenAbbr ="MSK";
  

    // mapping variable here
    mapping (address=> uint) public balances;


    // mint function
    function mint(address _address, uint _value) public{
        balances[_address]+= _value;
         totsupply += _value;
        ]

    // burn function
    function burn(address _address, uint _value) public{
        if(balances[_address]>=_value)
        {
        totsupply -= _value;
        balances[_address]-= _value;
        }
    }

}
```

## Executing program    
### How to Run the Program      
Navigate to the project directory  
Compile the Solidity contract  
Deploy the contract using your preferred Ethereum development environment   

#### For Remix:    
Open Remix IDE.  
Upload Token.sol.  
Compile and deploy the contract.  


## Any advise for common problems or issues.   
Ensure your Solidity compiler version matches the specified range.  
If you encounter issues with the compiler, try updating to a compatible version.  
Verify the Ethereum development environment is correctly set up.  

# Authors  
Muskan @Muskan5972

# License  
This project is licensed under the MIT License - see the LICENSE.md file for details.  

We have established a solidity contract with this code. 
