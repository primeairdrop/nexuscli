# Nexus Testnet II Prover Node 

## Step 1. Web Browser
Contribute to Nexus zkVM Prover : https://app.nexus.xyz/

Connect Wallet, Email (use same if did testnet 1) and copy your prover_id

## Step 2. Linux Server
- For Old User Do this step first
```console
rm -rf .nexus
```

---
*Install Dependencies*
```console
sudo apt update && sudo apt upgrade -y
```
```console
sudo apt install -y protobuf-compiler
```
```console
sudo apt install libssl-dev
```
```console
sudo apt install curl iptables build-essential git wget lz4 jq make gcc nano automake autoconf tmux htop nvme-cli pkg-config libssl-dev libleveldb-dev tar clang bsdmainutils ncdu unzip libleveldb-dev  -y
```
```console
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
- Click Enter to install default system settings
```console
source $HOME/.cargo/env
```
```console
export PATH="$HOME/.cargo/bin:$PATH"
```
```console
rustup target add riscv32i-unknown-none-elf
```
```console
sudo apt-get remove -y protobuf-compiler && wget https://github.com/protocolbuffers/protobuf/releases/download/v30.0-rc1/protoc-30.0-rc-1-linux-x86_64.zip && unzip protoc-30.0-rc-1-linux-x86_64.zip -d /usr/local/ && sudo chmod +x /usr/local/bin/protoc
```


*Open screen*
```console
sudo apt install screen
```
```console
screen -S nexus
```

*Run:*
```console
sudo curl https://cli.nexus.xyz/ | sh
```
- Enter prover id you copied from web browser
Error :
If facing error - Killed or memory allocation of 8606711792 bytes failed Aborted (core dumped)

*Run:*
```console
sudo fallocate -l 10G /swapfile && sudo chmod 600 /swapfile && sudo mkswap /swapfile && sudo swapon /swapfile && echo ‘/swapfile none swap sw 0 0’ | sudo tee -a /etc/fstab****
```
---
- Done | Feel free to ask queries in telegram channel
- Telegram - https://t.me/PrimeAirdrops_official
- Youtube - https://www.youtube.com/@primeairdrops6786
- Twitter - https://x.com/primeairdropsx
