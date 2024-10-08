# CLI PoP Miner
## Update
### 1. Remove old version
```Bash
rm -rf heminetwork_v0.4.3_linux_amd64 && rm -rf heminetwork
```
### 2. Download Binaries
```Bash
wget https://github.com/hemilabs/heminetwork/releases/download/v0.4.4/heminetwork_v0.4.4_linux_amd64.tar.gz
```
```Bash
tar xvf heminetwork_v0.4.4_linux_amd64.tar.gz && cd heminetwork_v0.4.4_linux_amd64
```
- To return screen
```Bash
screen -r hemi-pop
```
### 3. Replace your private key with <PRIVATE_KEY>
```Bash
echo 'export POPM_BTC_PRIVKEY=<PRIVATE_KEY>' >> ~/.bashrc
echo 'export POPM_STATIC_FEE=100' >> ~/.bashrc
echo 'export POPM_BFG_URL=wss://testnet.rpc.hemi.network/v1/ws/public' >> ~/.bashrc
source ~/.bashrc
```
### 4. Start your node
```Bash
./popmd
```
## ------DONE!---------------------------------------------------------------------------------------

## Install Miner on Linux
### 1. Download Binaries
```Bash
wget https://github.com/hemilabs/heminetwork/releases/download/v0.4.3/heminetwork_v0.4.3_linux_amd64.tar.gz
```
### 2. Extract Binaries
```Bash
tar xvf heminetwork_v0.4.3_linux_amd64.tar.gz && cd heminetwork_v0.4.3_linux_amd64
```
## Wallet
### 1. Create tBTC wallet
```Bash
./keygen -secp256k1 -json -net="testnet" > ~/popm-address.json
```
### 2. Get tBTC address
```Bash
cat ~/popm-address.json
```
### -Save you wallet
```Bash
  "ethereum_address": "0x123...",`
  "network": "testnet",`
  "private_key": "123...",
  "public_key": "123...",
  "pubkey_hash": "m12345..."
```
### 3. Fund your wallet
- Faucet tBTC: channel `#faucet` on Discord! type: `/tbtc-faucet address: <pubkey_hash>`
- Faucet HemiETF: channel `#faucet` on Discord! type: `/faucet address: <ethereum_address>`
## Start Miner
### 1. Create screen
```Bash
screen -S hemi-pop
```
### 2. Replace your private key with <PRIVATE_KEY>
```Bash
echo 'export POPM_BTC_PRIVKEY=<PRIVATE_KEY>' >> ~/.bashrc
echo 'export POPM_STATIC_FEE=100' >> ~/.bashrc
echo 'export POPM_BFG_URL=wss://testnet.rpc.hemi.network/v1/ws/public' >> ~/.bashrc
source ~/.bashrc
```
### 3. Start your node
```Bash
./popmd
```
- To detach from the screen session using `Ctrl + A + D`
- To return screen
  ```Bash
  screen -r hemi-pop
  ```

## 🎉 Congrats! You are now a Hemi PoP Miner!







