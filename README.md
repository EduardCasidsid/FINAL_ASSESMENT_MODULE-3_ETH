# FINAL_ASSESMENT_MODULE-3_ETH

This is the solidity that called mint and burn program, this program will show to you how to minting and how to burning the token and you will also know the total supply and value of the token

# Description

Our project is for MetaCrafters final assessment and for IT Elective 1 that will make a ethereum and create a mint and burn program and will know the total supply and value of the token.

# Getting Started

# Executing program

First search remix.etheruem.org then find the create a new file then name it want do you want like (stamptoken.sol) next put the code and put your choose name on token name and token abbrevation. when you finish the code, click remix compiler then compile your file and If you are finish compiling the code and click the deploy and run transactions then copy the link account and use it on the address of the burn ,mint and balances once you done putting the account of the address then add a value then transact first transact the mint to store the token then to burn the token just click the transact on the burn. And the value of mint is going to burn example you add a value of mint 1000 and put a value of burn 500 and click the token supply it will giving you a 500

//SPDX-License-Identifier: MIT pragma solidity ^0.8.18;

    contract metacrafters{

                 // public variables here
            string public TokenName = "Stamp Token";
            string public TokenAbbrv = "STP";
            uint public TotalSupply = 0;

                   // mapping variable here 
             mapping (address => uint) public Balances; 

                  // minting variable here
              function Minting (address Address, uint Value)public{
                        TotalSupply += Value;
                        Balances [Address] += Value;
                }
                  
                  // burning variable here
              function Burning (address Address, uint Value)public{
                       if(Balances[Address] >= Value){
                        TotalSupply -= Value;
                        Balances [Address] -= Value;}
               } 

    } 
# Help

The common error is missing symbol ;. Always check if there is an error per line, If there is an error your file name will turn red or the red symbol will pop up on the left side of the number it means there is an error.

;

# Authors

Eduard A. Casidsid 8213873@ntc.edu.ph

# License 

This project is licensed under the [MIT] License - see the LICENSE.md file for details
