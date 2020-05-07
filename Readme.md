# YoCoin Private Network

YoCoin was moved to Private Ethereum Network for more stability

## Installation on Ubuntu 16.04

Step 1: Environment configuration

```bash
mkdir yocoin && cd yocoin
```

Step 2: Getting Genesis state file 

```bash
wget 'https://raw.githubusercontent.com/Yocoin15/yocoin-privatenetwork/master/genesis.json'
```

Step 3: Installation of official Ethereum Geth Client

```bash
sudo add-apt-repository -y ppa:ethereum/ethereum && sudo apt-get update && sudo apt-get install ethereum
```

Step 4: Init your geth blockchain with YoCoin genesis data

```bash
geth --datadir "./datadir" init genesis.json
```

Step 5: Launch GETH Client (Example configuration)

```bash
geth --datadir "./datadir" --networkid 100892 --bootnodes "enode://34a45ad7e22ef272ab1b905dd7fa75c4b0d0618f36bbcdfeb1183b48cff42689b442246cc88f05a981e64de1c100d5a9d47933175cdb677c6a8fa5cd6996aeb5@139.59.21.215:30303"
```

### Private Network Data:
1. NetworkId = 100892
2. Bootnode = enode://34a45ad7e22ef272ab1b905dd7fa75c4b0d0618f36bbcdfeb1183b48cff42689b442246cc88f05a981e64de1c100d5a9d47933175cdb677c6a8fa5cd6996aeb5@139.59.21.215:30303
3. Geth client = latest on 6 May 2020



## Feedback
You can write to georgetagirov@gmail.com for any questions