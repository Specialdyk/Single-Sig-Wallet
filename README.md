# Single-Sig-Wallet
This contract allows a single owner to control and manage the funds stored within the wallet

The Single-Sig-Wallet Contract has an Owner Variable that stores the Ethereum address of the wallet's owenr. The contract is initalized with the depolyer of the contract becoming the owner.

The `onlyOwner` modifier ensures that only the owner can execute certain functions, it checks if the sender of the transaction (msg.sender) matches the owner's address.

The `depsoit` Function allows the people to depsoit ether to the wallet. Thsi is useful for funding the wallet.

The `Withdraw` Function allows the owner to withdraw Ether from the wallet provided they have sufficient balance.Only the owner can call this function.

The `getBalance` function allows anyone to check balance of the wallet.
