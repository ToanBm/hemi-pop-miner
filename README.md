# CLI PoP Miner

### 1. Binaries:
```Bash
wget https://github.com/hemilabs/heminetwork/releases/download/v0.4.3/heminetwork_v0.4.3_linux_amd64.tar.gz
tar xvf heminetwork_v0.4.3_linux_amd64.tar.gz && cd heminetwork_v0.4.3_linux_amd64
```
### 2. Generate Your Public Key:
```Bash
./popmd --help
```
```Bash
./keygen -secp256k1 -json -net="testnet" > ~/popm-address.json
```
```Bash
cat ~/popm-address.json
```
### - Save you Info:
```Bash
  "ethereum_address": "0x123...",`
  "network": "testnet",`
  "private_key": "123...",
  "public_key": "123...",
  "pubkey_hash": "m12345..."
```
### 3. Fund your PoP Miner Address:
- Faucet tBTC: channel `#faucet` on Discord! type: `/tbtc-faucet address: <pubkey_hash>`
- Faucet HemiETF: channel `#faucet` on Discord! type: `/faucet address: <ethereum_address>`
### 4.  Run the Miner:
```Bash
screen -S hemi-pop
```
### * Edit <private_key> 
```Bash
export POPM_BTC_PRIVKEY=<private_key>
export POPM_STATIC_FEE=500
export POPM_BFG_URL=wss://testnet.rpc.hemi.network/v1/ws/public
```
```Bash
./popmd
```
- To detach from the screen session using `Ctrl + A + D`

## 🎉 Congrats! You are now a Hemi PoP Miner!







