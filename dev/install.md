# Compile and Run

## Download
Download source code via `git`
```
    git clone https://github.com/omtch/omega-chain.git
```
## Install Golang
Reference: [Go Download and install](https://golang.org/doc/install)

## Compile
```
cd /path/to/omega-chain
make geth
```
> If you want to use cross compile, like compiling on `Mac` for `Linux`, use `make geth-linux`, `make geth-linux-amd64`, etc.


After compilation completed, the generated binary is in the folder `build/bin`.

## Run
By running `./build/bin/geth --help`, we can get all `option` info. Specific usage can refer to [Command-line Options](https://geth.ethereum.org/docs/interface/command-line-options)

## Deployment

please refer [deployment](/dev/deploy.md)

> SSD is required

