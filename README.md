# 🧩Nexus-L1
# Nexus Prover Node
You earn NEX Points by contributing compute and interacting with the Nexus ecosystem.

---

### Can I use multiple devices?
* Yes, you can connect as many devices as you want, including desktops, laptops, mobile phones, and servers
* You can link and manage all your devices from a single Nexus account
* You can also prove computations in multiple browser tabs simultaneously.

---
## --> Environments
  **You will need atleast 8GB of free ram**
  **You can run on both local pc/vps**
  
1- **Windows users**:
* Install **WSL (Windows Subsystem for Linux)**

2- **VPS users**:
* You can buy cheap VPS servers with good performance from anywhere

---

## --> Create account
* Create an account at https://app.nexus.xyz.

* Follow the account linking instructions.

* Your contributions will earn NEX Points.

* Track your progress on the leaderboard.

* Manage all your nodes in one place.

---

- You can run prover nodes on multiple browser tabs, desktops, laptops, mobile phones.
- Link and manage all your devices from a single Nexus account.
- **More computations = More NEX points**

---

## --> Contribute via CLI
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

#  Run Your Prover via CLI (Install via Script)

</div>



* Create screen session

```
screen -S nexus
```


* Install the Cli

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

Replace `<your-node-id>` with your actual node id



<div align="center">

#  Run Your Prover via CLI (Build from source)

</div>


* Create screen session

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

Replace `<your-node-id>` with your actual node id

You have succussfully run your Nexus prover node


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

Replace `<your-node-id>` with your actual node id

**Made with ❤️ by [Morsyxbt](https://x.com/morsyxbt)**
