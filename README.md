# Pre-compiled Cpuminer for Termux , Userland:
This is a WIP repo for pre-compiled cpuminer(v23.15) binary with Userland and GCC(v11.4.0).

# **`Disclaimer: I accept no warranties or liabilities on this repo. Do it at your own risk!!!`**

# **`This is for ARMv8`**

# Installation:
1. Download & install userland

2. Open Userland app and install Ubuntu accept permissions, we will use minimal environment and terminal or CLI this can take a couple minutes...
3. Get Ubuntu ready this can take a while:
- Type `y` then enter key in any prompts!
```
sudo apt update -y
sudo apt upgrade -y
sudo apt install git nano libcurl4-openssl-dev libjansson-dev -y
```
4. Download cpuminer, config, start:
```
git clone https://github.com/codlindor/cpuminer.git
cd cpuminer
chmod +x cpuminer start.sh
```
# Usage:

1. Edit your pool, address, worker name, your algo, etc....:
```
nano config.json
```
2. Start cpuminer with:
```
~/cpuminer/start.sh
```
3. Close cpuminer with:
```
CTRL + c
```
4. View more cpuminer commands with:
```
~/cpuminer/cpuminer -h
```
# Tips & Tricks:
- If having issues consider starting from scratch force close Userland then clear cache & data.
- Disable battery manager, battery optimization for Userland app.
- If you long press anywhere within Termux then click `More` there is an option to `Keep screen on`.
- Alternatively you can pull down the notification drawer and expand Userland notification to `Acquire wakelock` this will enable you to mine with the screen off **(NOTE! not all devices obey this rule is a hit or miss)**
- Use a pool with low latency to your location/internet.
- Give the miner/stratum time to stabilize hashrate(~30m-1h).
