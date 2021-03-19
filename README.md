# Neo 3 Hello Oracles sample contract

This is a sample [Neo 3](https://medium.com/neo-smart-economy/introducing-neo-n3-the-next-evolution-of-the-neo-blockchain-b2960c4def6e) blockchain smart contract,
demonstrating how to use [Neo-Express](https://github.com/neo-project/neo-express) and 
[Neo Smart Contract Debugger for Visual Studio Code](https://github.com/neo-project/neo-debugger) with oracles.

This sample is a basic "hello world" style contract. Building the contract will also build three neo-express checkpoints 

1. After sample contract has been deployed
2. After sample contract's `MakeOracleCall` operation is invoked
3. After neo-express `oracle response` command is run to respond to oracle request

> Note, as of Neo Express v2.0.18-preview, only `oracle response` command is supported for responding to oracle requests.
> A future version of Neo Express will support optional automatic oracle response processing, similar to how oracle requests are processed on production blockchains like MainNet.
