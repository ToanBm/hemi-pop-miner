# CLI PoP Miner

### 1. Binaries:
```Bash
wget https://github.com/hemilabs/heminetwork/releases/download/v0.3.13/heminetwork_v0.3.13_linux_amd64.tar.gz -O heminetwork_v0.3.13_linux_amd64.tar.gz
tar -xzf heminetwork_v0.3.13_linux_amd64.tar.gz
cd heminetwork_v0.3.13_linux_amd64
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
- Save you wallet:
```Bash
  "ethereum_address": "0x123...",`
  "network": "testnet",`
  "private_key": "123...",
  "public_key": "123...",
  "pubkey_hash": "m12345..."
```
### 3. Fund your PoP Miner Address:
- `#faucet` channel on Discord! type: `/tbtc-faucet address: <pubkey_hash>`
### 4.  Run the Miner:
```Bash
screen -S hemi-pop
```
```Bash
export POPM_BTC_PRIVKEY=<private_key>
export POPM_STATIC_FEE=150
export POPM_BFG_URL=wss://testnet.rpc.hemi.network/v1/ws/public
```
```Bash
./popmd
```
- To detach from the screen session using `Ctrl + A + D`

## 🎉 Congrats! You are now a Hemi PoP Miner!







