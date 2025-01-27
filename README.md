# T3rn_executor_node
Setting up T3RN Executor node on VPS

Welcome to t3rn, a Modular Interoperability Layer designed for fast, secure, and cost-efficient cross-chain swapping. t3rn is uniquely positioned to bridge the gaps in blockchain interoperability, offering superior swapping for users and yield for infra providers by becoming t3rn Executors.

Docs : [t3rn docs](https://docs.t3rn.io/intro) | X : [t3rn](https://x.com/t3rn_io)

---

# VPS Options

💻 Contabo VPS Deals 🚀 Buy with Credit Card/Paypal/Crypto Credit card : 

Get powerful VPS solutions with these direct links:  

| **VPS** | **Direct Link**                      | **Specs**                                                                          |
|---------|--------------------------------------|------------------------------------------------------------------------------------|
| VPS 1   | [Contabo VPS 1](https://www.jdoqocy.com/click-101278318-15692486) | 4 vCPU Cores, 4 GB RAM, 100 GB NVMe or 400 GB SSD     |
| VPS 2   | [Contabo VPS 2](https://www.anrdoezrs.net/click-101278318-13796472) | 6 vCPU Cores, 16 GB RAM, 200 GB NVMe or 400 GB SSD  |
| VPS 3   | [Contabo VPS 3](https://www.dpbolvw.net/click-101278318-13796474) | 8 vCPU Cores, 24 GB RAM, 300 GB NVMe or 1.2 TB SSD    |
| VPS 4   | [Contabo VPS 4](https://www.anrdoezrs.net/click-101278318-13796476) | 12 vCPU Cores, 48 GB RAM, 400 GB NVMe or 1.6 TB SSD |


💡 **Get started with the perfect VPS for your needs!** 🚀



⚠️ Important Notes
T3RN Swap and earn BRN https://bridge.t1rn.io

Check Executor https://bridge.t1rn.io/explorer/orders

BRN blockchain explorer https://brn.explorer.caldera.xyz

Minimum recommended Balance to run executor node:

🔴 L1RN = 1 BRN

🔴 ARB SEPO = 2 ETH

🔴 BASE SEPO = 2 ETH

🔴 OPT SEPO = 2 ETH

🔴 BLAST SEPO = 2 ETH

Bridge:

🔴 SEPO to ARB SEPO : https://bridge.arbitrum.io/?destinationChain=arbitrum-sepolia&sourceChain=sepolia

🔴 SEPO to BASE SEPO : https://superbridge.app/base-sepolia

🔴 SEPO to OPT SEPO : https://superbridge.app/op-sepolia

🔴 SEPO to BLAST SEPO : send Sepolia ETH to this address : 0xDeDa8D3CCf044fE2A16217846B6e1f1cfD8e122f to get ETH on Blast Sepolia

Faucet list:

🔴 https://faucet.quicknode.com/arbitrum/sepolia

🔴 https://faucets.chain.link/arbitrum-sepolia

🔴 https://bwarelabs.com/faucets/arbitrum-sepolia

🔴 https://www.alchemy.com/faucets/ethereum-sepolia

🔴 https://docs.metamask.io/developer-tools/faucet/

🔴 https://cloud.google.com/application/web3/faucet/ethereum/sepolia

ℹ️ You can also buy Sepolia ETH from TestnetBridge if you want to start quickly. 💡Arbitrum and OP networks gives best rates💡

👉 Official Discord Community
⚙️ This script will ask if you wan't to run API or RPC node.
ℹ️ API node = executor node will process requests from API and doesn't need to have a private Alchemy RPC points.
ℹ️ RPC node = executor will ask for Alchemy API key and will process only orders from RPC requests.
⚠️ Additionally script will ask if you want to add custom public RPC nodes. If you say NO then it will use default public RPCs which already integrated into script
✅ Select a node type

🔐 Input required details

🟠 Set Gwei, by default gwei is set for 200

🏃‍♂️‍➡️🏃‍♂️‍➡️🏃‍♂️‍➡️ Let it run! 🏃‍♂️‍➡️🏃‍♂️‍➡️🏃‍♂️‍➡️



----------------------------------------------------------------------------------------------------------------------------------------
### Getting Started with t3rn:
#### Participate as an Executor:
Join the network as an Executor to process transactions and engage in the ecosystem by bidding on orders and executing transactions.

#### Explore t3rn's Bridge UI:
Explore cross-chain swaps with our intuitive Bridge UI. Now live on testnets, it enables fast, secure, and cost-efficient cross-chain transactions.

Task : https://app.galxe.com/quest/t3rn/GC2NYtzDN6
[Answers : C, A, D, C]

Faucet : https://faucet.brn.t3rn.io/

Bridge : https://bridge.t1rn.io 

----------------------------------------------------------------------------------------------------------------------------------------

# Join Crypto WwCfAirdrops Community

Join TG : [Crypto WwCf Telegram](https://t.me/WwCfAirdrops) | Follow X : [Crypto WwCf Twitter](https://www.x.com/WwCfOfficial) | Subscribe : [Crypto WwCf Youtube](https://www.youtube.com/@WwCfOfficial)


----------------------------------------------------------------------------------------------------------------------------------------

### Update and upgrade system packages
```
sudo apt update
sudo apt upgrade
```
### Install fonts
```
sudo apt-get install figlet
figlet -f /usr/share/figlet/starwars.flf

```
### Download t3rn binaries
```
LATEST_VERSION=$(curl -s https://api.github.com/repos/t3rn/executor-release/releases/latest | grep 'tag_name' | cut -d\" -f4)
EXECUTOR_URL="https://github.com/t3rn/executor-release/releases/download/${LATEST_VERSION}/executor-linux-${LATEST_VERSION}.tar.gz"
curl -L -o executor-linux-${LATEST_VERSION}.tar.gz $EXECUTOR_URL

```
### Extract 
```
tar -xzvf executor-linux-${LATEST_VERSION}.tar.gz
rm -rf executor-linux-${LATEST_VERSION}.tar.gz
cd executor/executor/bin

```

### Open screen 
```
screen -S t3rn
```
### Set your preferred Node Environment.
```
export NODE_ENV=testnet
```
### Set your log settings
```
export LOG_LEVEL=debug
export LOG_PRETTY=false
export EXECUTOR_PROCESS_ORDERS=true
export EXECUTOR_PROCESS_CLAIMS=true
export EXECUTOR_MAX_L3_GAS_PRICE=50
export EXECUTOR_PROCESS_PENDING_ORDERS_FROM_API=false
```
### PRIVATE KEYS
Set the PRIVATE_KEY_LOCAL variable of your Executor, Replace with your privatekey
```
export PRIVATE_KEY_LOCAL=<replace your privatekey>
```
### Set Networks
```
export ENABLED_NETWORKS='arbitrum-sepolia,base-sepolia,optimism-sepolia,l1rn'
```
### Start Node
```
./executor
```

Take a screenshot of running node and post it on discord to get a role.


🎨 Understanding the Colors
The tool uses a variety of colors to make the output easy to read:


🟢 Green: Successful operations
🔵 Blue: General information
🟡 Yellow: Warnings or important notices
🔴 Red: Errors or failed operations
🟣 Magenta: Highlighted information
🟠 Cyan: Balance information




Done !! Feel free to ask queries in telegram channel

Telegram - https://t.me/WwCfAirdrops

Youtube - https://www.youtube.com/@WwCfOfficial

Credit: @WwCfOfficial