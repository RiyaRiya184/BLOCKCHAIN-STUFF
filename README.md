# BASIC COMMAND TO INSTALL GOLANG AND FABRIC

To update the system:-
                         
    sudo apt update

To install golang-go:-

    sudo apt install golang-go

To install docker:-

    sudo snap install docker

To install git:-

    sudo apt install git

To install fabric-samples:-

    git clone -b main https://github.com/hyperledger/fabric-samples.git

to install curl:-

    sudo apt install curl

To get in fabric-samples:-

    cd fabric-samples

To pull hyperledger docker image:-

    sudo bash
   
    curl -sSL https://bit.ly/2ysbOFE | bash -s

To get into test-network:-

    cd test-network

To up the network:-

    ./network.sh

    ./network.sh up

To create channel:-

    ./network.sh createChannel

To down the network:-

    ./network.sh down

![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/67c2b850a0cf4ac62700ff7f5e7fbc1039624eb0/madhu's%20terminal%20thing.png)

To install IPFS:-

    wget https://dist.ipfs.tech/kubo/v0.32.1/kubo_v0.32.1_linux-amd64.tar.gz

To use kubo:-

    tar -xvzf kubo_v0.32.1_linux-amd64.tar.gz

To get into kubo directory:-

    cd kubo

To move to local bin:-

    sudo bash install.sh

To initialise IPFS:-

    ipfs init
    
To use daemon:-

    ipfs daemon

![image alt]()

To run ipfs daemon in background:-

    ipfs.log 2>&1 &

To add file:-

    echo "Hello, IPFS!" > hello.txt
    ipfs add hello.txt
    ipfs cat <CID>

![image alt]()

To add a directory:-

    mkdir myfolder
    echo "File 1 content" > myfolder/file1.txt
    echo "File 2 content" > myfolder/file2.txt
    ipfs add -r myfolder

![image alt]()

lists running processes:-

    ps aux | grep ipfs

To kill the process:-

    kill <PID>

Encrypting and Decrypting:-

    echo "Hello, bruh" > myfile.txt
    ipfs add myfile.txt
    openssl enc -aes-256-cbc -pbkdf2 -iter 100000 -salt -in myfile.txt -out myfile_encrypted.txt -pass pass:yourpassword
    ipfs add myfile_encrypted.txt
    cat myfile_encrypted.txt
    openssl enc -d -aes-256-cbc -pbkdf2 -iter 100000 -in myfile_encrypted.txt -out decrypted_file.txt -pass pass:yourpassword
    cat decrypted_file.txt
    ipfs add decrypted_file.txt

![image alt]()

To add audio :-

    ipfs add <audio-path>

![image alt]()

To add video:-

    ipfs add <video-path>

![image alt]()

# Creating Meta Mask Account

The metamask account is our wallet where it store the token , like sepolia faucet which are the test token , with the help of metamask wallet we will do the transaction and deploy our smart contract on the blockchain.

![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/9f494403daf6d8688f7b2a3182fbfb44827773f0/ethirum%20wallet.png)

# Sepolia faucet

These are the test token because we can;t efford the etherum coin , also for the learning purpose we use them , these faucet can be get from the Google Cloud.

![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/915cab8228696c4a928dcbb4318c239ef51fcc66/google%20cloud%20sepolia.png)

Here in the above Image you can see the Wallet Address where we have to add the our metmask wallet address then click on the recive button and when you refresh your metamask account you can see the faucets.    

# Solidity:

We write our smart contract in the solidity language .

To use this Language I have used the Remix ide website where I can deploy my contract for free also we can use our metamask account to know how to make transcation through that.

![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/0413bf98b0cdea8d20b279bbce6b0a15e647eacd/remix%20ide%20front.png)
![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/73b46da0966bfb02b24fc19232d3e93a58f6ec2c/solidity1.png)

In above Image , the file explore saves our contracts.

Now we write a basic solidity code and try to compile run and deploy it

CODE:-

![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/4d4cbb14f8e41d0975d714504fbda6d69f759f6e/CODE.png)

Compiling the code:-

![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/017cdf53118278451a00c32cc2b192a7ca698aee/solidity%20compile.png)
![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/896dd311c590791c047da38e4c5e241c9be7f5d4/solidity%20compile%202.png)

Deploying on blockchain:-

![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/059067152642de55af3e52e3bb69e3125b8f3b46/deploy.png)

After Deploying we can see the green tick which show our contract is deployed on the blockchain

![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/413aa09e134a9e2ad13931cbfa343deaec84cd88/running%20the%20code.png)

Running the code:-

![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/67ebe8f809b4bc98382aa83b45534e0682016555/running%20of%20code2.png)

# practical questions

**question 1:Create a voting system with multiple candidates. Each address can vote only once.** 

![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/c07e89b5af7d220f5cb9e4c907a24ecf9716f8e3/code%201.png)
![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/4499963b59753f6ebb7da338b78fc97c55a874af/tr%201.png)

**Question 2:Write a contract that manages a list of student records (name, roll number). Allow adding and retrieving student data.**

![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/6b2fd45f3e6b31e96bd85ac6309990631e21a849/code2.png)
![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/0fa9bd501906634fde0672728255b62dcee4d0a1/tr2.png)

**Question 3:Develop a contract that only allows the deployer (owner) to call a specific function (use modifiers).**

![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/273a05a35d3bc321bf5ab3bacd67dcd34137f2c0/code%203.png)
![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/c6ad50acc671891a2f97ae010f8c7c4d151b589b/tr3.png)

**Questin 4:Write a contract where people can donate Ether and the top 3 donors are tracked.**

![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/73d4160fa891d2ec5ad55360a75786b203c344d5/code4.2.png)
![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/eac95e4c0a32ccdcef278ddc57e430f5efa91d28/tr4.2.png)

**Question 5:Implement a simple auction system where users can place bids, and the highest bidder wins.**

![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/e488a09619d00eef5653d03c47d5cb80a7eddd90/code%205.png)
![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/40d771394d467b980616672ac5a0160dadb58230/tr%205.png)

**Question 6:Create a contract that splits incoming Ether between 3 fixed addresses.**

![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/d94195e6bf3722cef80e40c03977442155ba9827/code%206.png)
![image alt](https://github.com/RiyaRiya184/BLOCKCHAIN-STUFF/blob/2c06e3182f758937ad7499ed21e61b4dc2f807ea/tr6.png)


