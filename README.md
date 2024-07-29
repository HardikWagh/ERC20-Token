# ERC20-Token
This repository contains the solidity smart contract for ERC20 Token
The Algorithm for the contract is as follows:

1. Define ERC20 Interface:
    -Declare functions for "totalSupply", "balanceOf", "allowance", "transfer", "approve", and "transferFrom".
    -Declare events for "Transfer" and "Approval".
2. Define Token Contract:
    -Define token attributes: "symbol", "name", "decimals", and "_totalSupply".
    -Create mappings for balances and allowances.
3. Constructor:
    -Set token attributes.
    -Initialize total supply and assign it to a specific address.
    -Emit "Transfer" event for initial supply assignment.
4.Implement Functions:
    -totalSupply: Return the total token supply excluding tokens held at the zero address.
    -balanceOf: Return the token balance of a specific address.
    -transfer: Transfer tokens from the sender to a recipient.
        -Update balances.
        -Emit "Transfer" event.
    -approve: Approve an allowance for a spender.
        -Update the allowance mapping.
        -Emit "Approval" event.
    -transferFrom: Transfer tokens from a sender to a recipient using an allowance.
        -Update balances and allowances.
        -Emit "Transfer" event.
    -allowance: Return the remaining allowance for a spender.
