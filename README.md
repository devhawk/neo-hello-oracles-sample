# Neo N3 Hello Oracle Smart Contract Sample

This is a sample [Neo N3](https://medium.com/neo-smart-economy/introducing-neo-n3-the-next-evolution-of-the-neo-blockchain-b2960c4def6e) blockchain smart contract,
demonstrating how to use [Neo-Express](https://github.com/neo-project/neo-express) and 
[Neo Smart Contract Debugger for Visual Studio Code](https://github.com/neo-project/neo-debugger) with oracles.

This sample is a basic "hello world" style contract. Building the contract will also build three neo-express checkpoints 

1. After sample contract has been deployed
2. After sample contract's `MakeOracleCall` operation is invoked
3. After neo-express `oracle response` command is run to respond to oracle request

> Note, as of Neo Express v2.0.21-preview, only `oracle response` command is supported for responding to oracle requests.
> A future version of Neo Express will support optional automatic oracle response processing, similar to how oracle requests are processed on production blockchains like MainNet.

## Prerequisites

> Note, if you're using [VS Code Remote Container](https://code.visualstudio.com/docs/remote/containers)
  or [GitHub Codespaces](https://github.com/features/codespaces),
  the [devcontainer Dockerfile](.devcontainer/Dockerfile) for this repo has all the prerequisites installed.

- [.NET 5.0 SDK](https://dotnet.microsoft.com/download/dotnet/5.0)
- [Visual Studio Code (v1.52 or later)](https://code.visualstudio.com/Download)

### Ubuntu Prerequisites

Installing on Ubuntu 18.04 or 20.04 also requires installing libsnappy-dev and libc6-dev
via apt-get. 

``` shell
$ sudo apt install libsnappy-dev libc6-dev -y
```

### MacOS Prerequisites

Installing on MacOS requires installing rocksdb via [Homebrew](https://brew.sh/).

``` shell
$ brew install rocksdb
```

