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
### 1. Install Dependecies
```bash
sudo apt update & sudo apt upgrade -y
sudo apt install screen curl build-essential pkg-config libssl-dev git-all -y
sudo apt install protobuf-compiler -y
sudo apt update
```
```bash
curl --proto '=https' --tlsv1.2 -sSf https://sh.rustup.rs | sh
```
```bash
source $HOME/.cargo/env
```
```bash
rustup target add riscv32i-unknown-none-elf
```

---

### 2. Run Prover
**1- Start a screen to keep it running in the background**
```bash
screen -S nexus
```
**2- Install and run prover**
```bash
curl https://cli.nexus.xyz/ | sh
```

**3- Run with an existing node ID**

```
source ~/.bashrc
```
```
nexus-network start --node-id your-node-id
```
* Replace `your-node-id` with the one acquired in the next step.

---

### 3. Create Node ID
* ---> **Create Node ID via Web:**

1- Go to https://app.nexus.xyz/nodes

2- Click `Add Node`, click `Add CLI Node` and copy your `node-id` and paste in terminal

---

### Earn more NEX? Run Multiple CLI Nodes:
Now you can create more Node sessions by creating more screens. for example, to create the 2nd node:
* Create 2nd screen:
```
screen -S nexus2
```

* Create 2nd node ID:
```
nexus-network register-node
```

* Run 2nd Node with 2nd Node ID:
```
nexus-network start --node-id your-node-id
```
* Replace `your-node-id` with the newly created one

**Note**: Monitor your server's RAM and CPU via `htop` command to see how many nodes you can run
```console
# install htop
sudo apt install htop

# run htop
htop
```

---

### 4. Manage your Node screen:
* To minimze the screen: `CTRL+A+D`

* To return to screen: `screen -r nexus`

* To kill screen: `screen -XS nexus quit`

---

## **Made with ❤️ by Morsyxbt
