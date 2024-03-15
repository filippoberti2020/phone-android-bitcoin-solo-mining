# Phone android bitcoin solo mining GUIDE

## How to Mine Solo on Android Devices

1. **Download Termux**: [Termux F-Droid](https://f-droid.org/en/packages/com.termux/)

### Inside Termux App use the following commands:

2. `termux-setup-storage`
3. `apt-get update`
4. `apt-get upgrade -y`
5. `apt-get install wget -y`
6. `apt-get install openssl-tool -y`
7. `apt-get install proot -y`
8: `wget https://raw.githubusercontent.com/EXALAB/AnLinux-Resources/master/Scripts/Installer/Ubuntu/ubuntu.sh && bash ubuntu.sh`
9: `./start-ubuntu.sh ; su`
10: `apt-get update`
11: `apt-get upgrade -y`
12: `apt install git -y`
13: `apt install proot -y`
14: `apt-get install automake autoconf pkg-config libcurl4-openssl-dev libjansson-dev libssl-dev libgmp-dev zlib1g-dev make g++ 
(Y and press enter, or press enter with Y selected if confirmation is requested.)`
15: `git clone https://github.com/tpruvot/cpuminer-multi`
16: `cd cpuminer-multi`
17: `./build-linux-arm.sh`
18: Start cpuminer :

`./cpuminer -o stratum+tcp://pool.vkbit.com:3333 -u <bitcoinaddress>.<workername> -p x -a sha256d -R 10`

Or with tread limitation ( -t 2 ) how many threads

`./cpuminer-o stratum+tcp://pool.vkbit.com:3333 -u <bitcoinaddress>.<workername> -p x -a sha256d -R 10 -t <threadsnumber>`

App can run in background, if you want to quit press CTRL + c
