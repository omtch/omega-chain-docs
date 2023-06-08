# Mainnet Info

## chainid
```
    408
```
## rpc

```
    https://mainnet-rpc.omtch.com
```

## explorer
```
    https://explorer.omtch.com
```

# P2P Nodes

allow P2P port（default 32668） udp/tcp

```
enode://6197dab4973bfae9041efe1c4f77e98a3e6a7a1239036231d8d3a702261842b7b43b81b515d9c0382486c376c45b0f2d1acb6e8383d5187c422cd9a3d1533999@34.133.149.176:32668

enode://7ef76a16ad557e74cd183ac81c39d5388e82ea2775b18dc1ee67831cca75391bfea654ccb3edacfc608fa60ab5ed77c3a378383654a9ac3397db2839b384cc6c@34.92.28.33:32668
```


put below into static node：

```
[Node.P2P]

StaticNodes = [
    "enode://6197dab4973bfae9041efe1c4f77e98a3e6a7a1239036231d8d3a702261842b7b43b81b515d9c0382486c376c45b0f2d1acb6e8383d5187c422cd9a3d1533999@34.133.149.176:32668",
    "enode://7ef76a16ad557e74cd183ac81c39d5388e82ea2775b18dc1ee67831cca75391bfea654ccb3edacfc608fa60ab5ed77c3a378383654a9ac3397db2839b384cc6c@34.92.28.33:32668"
]
```