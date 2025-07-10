<div align="left">

#   **Introduction📔**

</div>

-----Nexus is a next-generation Layer 1 blockchain designed as a global, verifiable supercomputer for the AI era. It enables decentralized, trustless computation using zero-knowledge proofs via its custom zkVM. Developers and users can contribute compute power and earn rewards. The platform is open-source, EVM-compatible, and built to power scalable AI and smart contract applications.


<div align="center">

#  👨🏻‍💻 **Nexus Prover Node Guide** 👨🏻‍💻

</div>


# Device/System Requirements 💻

* So Minimun 12GB of memory can we sufficient for running a Nexus Prover node, 

* You can run multiple nodes in a single vps/device: But **I wont recommend it** cause If u dont have sufficient memory then it can be cause of **system crash**:❗❗

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
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```

```
source $HOME/.cargo/env
```

Check version

```
rustc --version
```


<div align="center">

#  Run Your Prover via CLI (Install via Script) 🍥

</div>



* Create screen session (Vps Only)

```
screen -S nexus
```


* ####  Install the Cli

```
curl https://cli.nexus.xyz/ | sh
```

* Add nexus to your path

```
source ~/.bashrc
```

* **Start Your Prover**

```
nexus-network start --node-id <your-node-id>
```

Replace `<your-node-id>` with your actual node id from [Get your node ID 🛠](https://github.com/Mayankgg01/Nexus_Prover_Node_Guide/tree/main?tab=readme-ov-file#get-your-node-id-)



<div align="center">

#  Run Your Prover via CLI (Build from source) 🍥

</div>


* Create screen session (Vps Only)

```
screen -S nexus
```

* Clone the Repository


```
git clone https://github.com/nexus-xyz/nexus-cli.git
```

* Move & Build the release

```
cd ~/nexus-cli/clients/cli
```

```
cargo build --release
```


🔺It will take some time here to compile it:


* Add nexus to your path

```
source ~/.bashrc
```


* **Start Your Prover**

```
cargo run -r -- start --node-id <your-node-id>
```

Replace `<your-node-id>` with your actual node id from [Get your node ID 🛠](https://github.com/Mayankgg01/Nexus_Prover_Node_Guide/tree/main?tab=readme-ov-file#get-your-node-id-)




![image](https://github.com/user-attachments/assets/a2c9bb37-e72b-4c42-8d7a-14554de938e5)


Here we go: You have succussfully run your Nexus prover node🚀😙


# Detach & Attach from screen

`ctrl` `A` `D` To Detach from screen 

* Attach with previous screen:


`screen -ls` to know about the screens:

Attach with this command:

`screen -r Screen_Name` 



* U can check Memory on your VPS by this command:

```
free -h
```


# Next Day start command for local PC:

* Just run the start prover command:

```
nexus-network start --node-id <your-node-id>
```

Replace `<your-node-id>` with your actual node id from [Get your node ID 🛠](https://github.com/Mayankgg01/Nexus_Prover_Node_Guide/tree/main?tab=readme-ov-file#get-your-node-id-)



<div align="center">

# 📈 Upgrade to new release {v0.9.0}     (Mac/Linux)

</div>


### If you have followed [Run Your Prover via CLI (Install via Script) 🍥](https://github.com/Mayankgg01/Nexus_Prover_Node_Guide?tab=readme-ov-file#run-your-prover-via-cli-install-via-script-) then follow these process 👇


* You Just have to follow from here [Install the Cli](https://github.com/Mayankgg01/Nexus_Prover_Node_Guide/tree/main?tab=readme-ov-file#install-the-cli) Thats it!





### If You have followed [Run Your Prover via CLI (Build from source) 🍥](https://github.com/Mayankgg01/Nexus_Prover_Node_Guide?tab=readme-ov-file#run-your-prover-via-cli-build-from-source-) then follow these process 👇



* Move to Directory

```
cd ~/nexus-cli
```

* Pull the latest Release

```
git fetch --tags
git checkout tags/v0.9.1
```

* Build the release

```
cargo build --release
```

```
source ~/.bashrc
```

* Start Your prover:

```
cargo run -r -- start --node-id <your-node-id>
```

Dont Forget to Replace Your Node-Id

All Set!✔️


👉 Join TG for more Updates: https://telegram.me/cryptogg

If U have any issue then open a issue on this repo or Dm me on TG~

💗Thank You! Happy Coding!📈
