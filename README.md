# Howto Install EOS node:  
  

mkdir /home/eos-dawn-v3.0.0  
cd /home/eos-dawn-v3.0.0  

### Clone into new folder
```console
cd /opt
git clone https://github.com/eosio/eos --recursive
```
### Checkout master branch and update submodules
```console
cd eos
git checkout master
git pull
git submodule update --init --recursive
```

### Build and install
```console
./eosio_build.sh
cd build
make install
```

# How to configure node and test BP
- Create data-dir folder for you node:
  mkdir /opt/EOS-Pacific-Rim
- Download files config.ini, genesis.json, start.sh, stop.sh and put in this folder /opt/EOS-Pacific-Rim
- All paths in files are binded to this data folder
- add execution rights  
  chmod 777 /opt/EOS-Pacific-Rim/*.sh  
  
- Choose your producer name (any jungle animal ;) and create own EOS key pair  
  you can create key pair using cleos command ./cleos create key or <a target="_blank" href="https://nadejde.github.io/eos-token-sale/">here</a>.
- Edit config.ini with your producer name and created key pair
- Open http and p2p Ports on your firewall/router
- Connect your node, run ./start.sh
- Check if you can access you node using link http://you_server:your_http_port/v1/chain/get_info (<a href="http://jungle.cryptolions.io:8888/v1/chain/get_info" target="_blank">Example</a>)

- if your node is connected and synced -  **Send Request** in <a target="_blank" href="https://t.me/jungletestnet">telegram channel</a> with next information:  
    
| Server Location | Organisation | node ip/domain, | Port (http) |  Port (p2p) | producer name | your public key|
|-----------------|--------------|-----------------|-------------|-------------|---------------|----------------|

  
  


# BP Nodes Information
| BP Name | Address | Port (http) | Port (p2p) | Location | Organisation |
|---------|---------|-------------|------------|----------|--------------|
| Volcano | jungle.cryptolions.io | 8888	| 9876	 | Ukraine, Kyiv | CryptoLions.io |
| EOS Beijing | 150.109.65.114 | 8888	| 9876 | Hongkong | EOS Beijing |



# Nodes
| Address | Port (http) | Port (p2p) | Location | Organisation |
|---------|-------------|------------|----------|--------------|



# Nodes waiting to be connected
| BP Name | Address | Port (http) | Port (p2p) | Location | Organisation |
|---------|---------|-------------|------------|----------|--------------|


