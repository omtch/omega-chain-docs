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

```
./geth --datadir data/ init testnet-genesis.json

./geth --syncmode full --datadir data --http --http.addr 0.0.0.0 --http.port 8545 --http.corsdomain=* --http.vhosts=* --http.api personal,db,eth,net,web3,txpool,miner --ws --ws.addr 0.0.0.0 --ws.port 8546 --ws.origins=* --ws.api personal,admin,db,eth,net,web3,miner,shh,txpool,debug --gcmode=archive --bootnodes "enode://6a17ac142d7ae2b7e41ff85734f9b22f2886674ade653ca4d65a48546b70471b1d4aa179f4d7348e3b97ea43f65759c0bcb1021cebadb15c092f78e3dc74c830@10.170.0.7:32668"
```

> SSD is required
