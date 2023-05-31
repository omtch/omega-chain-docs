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
// TESNET

./geth --datadir data/ init testnet-genesis.json

./geth --syncmode full --datadir data/ --http --http.addr 0.0.0.0 --http.port 8545 --http.corsdomain=* --http.vhosts=* --http.api personal,db,eth,net,web3,txpool,miner --ws --ws.addr 0.0.0.0 --ws.port 8546 --ws.origins=* --ws.api personal,admin,db,eth,net,web3,miner,shh,txpool,debug --gcmode=archive --bootnodes enode://163fcba9e550fb31baf895153111fc212a2ef73ca904c4437cf164f69f0a2046b5b2090d2a7ab2dcec9dbc1e9787bb94468c39b7ea1c56dfb55664971924e47b@34.64.149.189:32668
```

> SSD is required
