# Welcome to the Advantage Daemon Download for Linux
# the Daemon is a Non-GUI Interface Used to for Masternodes 


Instructions:

1. Install dependencies

sudo apt-get install git
 
sudo apt-get install build-essential libtool autotools-dev automake pkg-config libssl-dev libevent-dev bsdmainutils
 
sudo apt-get install libboost-system-dev libboost-filesystem-dev libboost-chrono-dev libboost-program-options-dev libboost-test-dev libboost-thread-dev
 
sudo apt-get install libboost-all-dev
 
sudo apt-get install software-properties-common
 
sudo add-apt-repository ppa:bitcoin/bitcoin
 
sudo apt-get update
 
sudo apt-get install libdb4.8-dev libdb4.8++-dev
 
sudo apt-get install libminiupnpc-dev
 
sudo apt-get install libzmq3-dev
 
sudo apt-get install libqt5gui5 libqt5core5a libqt5dbus5 qttools5-dev qttools5-dev-tools libprotobuf-dev protobuf-compiler
 
sudo apt-get install libqt4-dev libprotobuf-dev protobuf-compiler

2. Download daemon using: git clone https://github.com/advantage-development/linux16.04-daemon
3. Open Port(11235) and Rpcport(53211)
4.  type the following commands
 sudo apt-get update
 sudo apt-get install ufw
 sudo ufw allow ssh/tcp
 sudo ufw limit ssh/tcp
 sudo ufw allow 53211/tcp
 sudo ufw allow 11235/tcp
 sudo ufw logging on
 sudo ufw enable
 sudo ufw status
 5. type cd .Advantage && nano Advantage.conf
 6. type in the following details
 
  server=1
  rpcuser=yourusername
  rpcpassword=yourpassword
  rpcport=53211
  listen=1
  server=1
  daemon=1
  logtimestamps=1
  maxconnections=256
