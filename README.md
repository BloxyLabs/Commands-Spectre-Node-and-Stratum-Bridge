# Commands-Spectre-Node-and-Stratum-Bridge

Here you can find the commands used in the BloxyLabs video about setting up a Spectre Node and Spectre Stratum Bridge
<br>
<br>
Check also our YouTube channel for instructions and other related information [YouTube](https://www.youtube.com/@bloxylabs "YouTube").
<br>
If you had fun with the projects, please consider giving us a Super Thanks on YouTube or buying us a [cup of coffee](https://www.buymeacoffee.com/bloxylabs "cupofcoffee").

**Command to upgrade the OS:**

```
sudo apt upgrate
```

**Command to install wget if it is not installed on your OS:**

```
sudo apt install wget
```

**Command to download the full node software:**

```
wget https://github.com/spectre-project/rusty-spectre/releases/download/v0.3.16/rusty-spectre-v0.3.16-linux-gnu-aarch64.zip
```
Always check the Spectre Network GitHub for the latest version.

**Command to unzip:**

```
unzip NAMEOFTHEFILEYOUWANTTOUNZIP
```

**Command to start the node:**

```
./spectred --utxoindex --rpclisten=0.0.0.0:18110
```
Be sure you are in the bin directory.

**Command to download the Spectre Stratum Bridge:**

```
wget https://github.com/spectre-project/spectre-stratum-bridge/releases/download/v0.3.17/spr_bridge-v0.3.17-linux-aarch64.zip
```
Always check the Spectre Network GitHub for the latest version.

**Command to edit the config file:**

```
nano config.yaml
```
Be sure you are in the bin directory of the downloaded and extracted Stratum Bridge files. Change localhost behind spectred_address on 0.0.0.0

**Command to start the Spectre Stratum Bridge :**

```
./spr_bridge
```

**Commands to install screen and start a screen session:**

```
sudo apt-get install screen
```
```
screen
```
Type ctrl-a and d to detach from a screen session and use the command screen-r to reattach to the session.

**Command to start the miner:**

```
./tnn-miner-cpu --daemon-address IPADDRESSOFYOURNODE --port 5555 --wallet WALLETADDRESS.WORKERNAME --threads 8
```
Use 8 threads for the Orange Pi 5 and 4 threads for the Raspberry Pi 5
