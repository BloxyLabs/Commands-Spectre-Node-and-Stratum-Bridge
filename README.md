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

**Command download the full node software:**

```
wget https://github.com/spectre-project/rusty-spectre/releases/download/v0.3.16/rusty-spectre-v0.3.16-linux-gnu-aarch64.zip
```
Always check the Spectre Network GitHub for the latest version

**Command to unzip:**

```
unzip NAMEOFTHEFILEYOUWANTTOUNZIP
```

**Command to run the node:**

```
./spectred --utxoindex --rpclisten=0.0.0.0:18110
```
Be sure you are in the bin directory.

**Command to download the Spectre Stratum Bridge:**

```
wget https://github.com/spectre-project/spectre-stratum-bridge/releases/download/v0.3.17/spr_bridge-v0.3.17-linux-aarch64.zip
```
Always check the Spectre Network GitHub for the latest version

**Command to download the TNN Miner file from GitLab:**

```
wget https://gitlab.com/Tritonn204/tnn-miner/-/releases/0.4.3-r2/downloads/Tnn-miner-arm64-0.4.3-r2.tar.gz
```
Always check the gitlab if there are newer versions.

**Command to extract a tar.gz file:**

```
tar -xvzf FILENAME.tar.gz
```
Command from the video:
```
tar -xvzf Tnn-miner-arm64-0.4.3-r2.tar.gz
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
./tnn-miner-cpu --daemon-address spr.tw-pool.com --port 14001 --wallet WALLETADDRESS.WORKERNAME --threads 8
```
Use 8 threads for the Orange Pi 5 and 4 threads for the Raspberry Pi 5
