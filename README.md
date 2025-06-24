<div align="left">

#   **Introduction📔**

</div>

-----Nexus is a next-generation Layer 1 blockchain designed as a global, verifiable supercomputer for the AI era. It enables decentralized, trustless computation using zero-knowledge proofs via its custom zkVM. Developers and users can contribute compute power and earn rewards. The platform is open-source, EVM-compatible, and built to power scalable AI and smart contract applications.


<div align="center">

#  👨🏻‍💻 **Nexus Prover Node Guide** 👨🏻‍💻

</div>


# Device/System Requirements 💻

* So Minimun 4GB of memory can we sufficient for the Nexus Prover, 

* And u can run multiple nodes in a single vps/device:

* **More Memory/RAM = High Cycles/sec**

# Get your node ID 🛠


* Register on web> https://app.nexus.xyz/nodes
* Go to Nodes>
* Add Cli Node> 
* Get your node Id


# Install All Require Dependecies


```
sudo apt-get update && sudo apt-get upgrade -y
```

```
sudo apt install curl iptables build-essential git wget lz4 jq make cmake gcc nano automake autoconf tmux htop nvme-cli libgbm1 pkg-config libssl-dev libleveldb-dev tar clang bsdmainutils ncdu unzip libleveldb-dev screen ufw -y
```

* Install rustup

```
curl https://sh.rustup.rs -sSf | sh
```

```
source $HOME/.cargo/env
```

Check version

```
rustc --version
```


<div align="center">

#  Run Your Prover by CLI 🍥

</div>




* Create screen session (Vps Only)

```
screen -S nexus
```


* Install the Cli

```
curl https://cli.nexus.xyz/ | sh
```

* Add nexus in your path

```
source ~/.bashrc
```

* **Start Your Prover**

```
nexus-network start --node-id <your-node-id>
```

Replace `<your-node-id>` with your actual node id from [Get your node ID 🛠](https://github.com/Mayankgg01/Nexus_Prover_Node_Guide/edit/main/README.md#get-your-node-id-)


![image](https://github.com/user-attachments/assets/a2c9bb37-e72b-4c42-8d7a-14554de938e5)


Here we go: You have succussfully run your Nexus prover node🚀😙


# Detach & Attach from screen

`ctrl` `A` `D` To Detach from screen 

* Attach with previous screen:


`screen -ls` to know about the screens:

Attach with this command:

`screen -r Screen_Name` 


# Run Multiple Prover node in a single vps/device

* Create another Screen 

```
screen -S nexus2
```

* Get node if from here: Generate New: [Get your node ID 🛠](https://github.com/Mayankgg01/Nexus_Prover_Node_Guide/edit/main/README.md#get-your-node-id-)

* **Start your prover**

```
nexus-network start --node-id <your-node-id>
```

Replace `<your-node-id>` with your actual node id:


❗❗**Note**:  Depend on your system/Vps u can run multiple nodes: Dont cross the limit and monitor your memory uses and cpu before doing multiple:




# Next Day start command for local PC:

* Just run the start prover command:

```
nexus-network start --node-id <your-node-id>
```

Replace `<your-node-id>` with your actual node id from [Get your node ID 🛠](https://github.com/Mayankgg01/Nexus_Prover_Node_Guide/edit/main/README.md#get-your-node-id-)



👉 Join TG for more Updates: https://telegram.me/cryptogg

If U have any issue then open a issue on this repo or Dm me on TG~

💗Thank You! Happy Coding!📈
