# Blockchain-Homework-Columbia-FinTech-Boot-Camp

## blockchain-homework
# Instructions
0. Allocate a few hours of focus. 
1. Ensure that you have downloaded and installed anaconda, puppeth, geth, and MyCrypto. You will need these tools in order to access ZBank's blockchain network and crypto wallet.
1. Open your Terminal and set your virtual environment to "zbank" with the command: conda activate zbank
2. Direct to the folder in which you have geth saved
3. To initialize the first node on the blockchain, run the command: ./geth init z.json --datadir znode1 (taken from class)
4. To initialize the first node on the blockchain, run the command: ./geth init z.json --datadir znode2 (taken from class) 


6. Create a file or note called "passwords or whatever" with the password for the node(s), and save it in the same directory as your node files
7. To start mining the first node, run the command: ./geth --datadir znode1 --mine --minerthreads 1 --rpc --unlock "0xF17375541F837a2F2a99d9eF38B9CbE6c8832ed3" --allow-insecure-unlock --password
8. The --mine flag tells the node to mine new blocks.
9. The --minerthreads flag tells geth how many CPU threads, or "workers" to use during mining. 
10. The --unlock flag unlocks the node for use - the  value calls the file we created above
11. The --allow-insecure-unlock flag allows us to unlock in an insecure mananer
12. The --rpc flag allows this node to communciate via the internet
13.  To start mining the second node, run the command: ./geth --datadir znode2 --port 30304 --bootnodes "enode://ba0824d777e04010d33441cccf4dd721115f081a555e331fc8c745b55f734254e932c60aef17034ac33807eeaef40b546db6b0f11e1125f6a9994ca74829edbb@127.0.0.1:30303"

# My Crypto Wallet application

15. Open the MyCrypto app and login to your account- set up an account, do what you need to do to have an account 
16. You will need to tap into the test network, in order to set this up on your app, please configure as shown in the "network-config" image in "Screenshots" folder in github.
Once you have set up the network on your app, go to "View & Send" in the top left, and choose "Keystore File" as your authentication method. This will prompt you to direct to the file path of one of the crypto wallets below on your device. Select the file, and enter the password when prompted (also listed below).

You should now be in the wallet. In order to send ETH to the other account you are not currently in, copy and paste the receiving account's public key from below into the "To Address" input box, choose how much ETH you would like to send, and click on "Send Transaction"

Celebrate, You are rich bish! go buy a g-wagon. 



# Network Information
## Network Name: zbank
## Chain ID: 510

# Accounts:
znode1 ** password = Mlark94 ** Public address of the key: 0xF17375541F837a2F2a99d9eF38B9CbE6c8832ed3 ** Path of the secret key file: znode1/keystore/UTC--2020-05-03T02-32-05.598612000Z--edf2ac0d77a16b4e1dd17224129cdcf1e0525a29 ** Port: 30303

znode2 ** password = Mlar94 ** Public address of the key: 0x03edDCd87cfB9aCaa608911fdCF6bfE43F08B93a ** Path of the secret key file: znode2/keystore/UTC--2020-05-03T02-32-38.828197000Z--376454e075d4beb0cd60e42001ea85d0de33acc8 ** Port: 30304
