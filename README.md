# BlackDiamondSCIncDAT

Installation: $npm install -g ganache-cli 

2. Metamask Extension : This is undoubtedly the most imperative requirement since it helps us to access Ethereum enabled distributed application(DAPPs) in your normal browsers like Firefox or Chrome. 

Get Metamask Extension here: https://metamask.io/ 

3. Truffle : This is the best development tool out there that includes all the necessary files and environment you might for not only deploying and developing your smart contracts but also testing it. 

Installation : $npm install -g truffle 

LET’S FINALLY CONNECT 

Now considering you managed to install all the prerequisites successfully, let’s now connect our smart contract to front-end. 

Although there is a variety of frameworks you may choose to develop the front end, as of now, let’s go with react. 

Well, there is no deny in the fact that considering the complexity of React itself, it might be troublesome to write all the code from scratch. Well, truffle has got your back here as it provides you with some boiler plate code that connects the React to Web3. All you have to do is to install the truffle’s react box. 

Install: $truffle unbox react 

STEP 1: 

Edit Truffle-config.js : Once you unbox the react component from truffle, the first job is to edit the network object in the module.export section. Set the host to localhost and port to 8545. 

Why Do This? 

Well, we need to connect our dapp to a local blockchain. And in our case, Ganche CLI is going to do that job. And most importantly, Ganache CLI listens to port 8545, which is why we set our port to 8545 in the tuffle.js. 

STEP 2: 

Initiate Ganache CLI : The next part is to run the command ganache-cli your terminal to activate Ganache.


Note: Ganache CLI is listening to port 8545. 

STEP 3: 

Setting Up METAMASK: 

Truth be told, this is the part where things might turn out to be ugly. Therefore, let’s understand the very basics of this step. 

Metamask can simply be seen as a tool that basically transforms your normal browser, i.e., Firefox or Chrome, into the ones that can talk to the blockchain. 

While developing this can be done by providing suitable port to this metamask extension and setup its connection with our development account. 

And for that, you have two reliable ports for development purposes. 

Port 7545 :- While working with Ganache GUI 

Port 8545 :- While working with Ganche CLI 

So, assuming you successfully established the Metamask extension on your favorite browser, now let’s begin with the main part. 

As you see, by default, this extension is connected to the Main Ethereum Network, which is not all the account you want to use for development purposes(unless you are really rich and own lots of ether). So Click on the drop-down menu and select Localhost 8545.(because Ganache CLI is using the port 8545). 

Once the port is set, now click on the circular button on the top right portion and select the Import Account option. 

Here you will be asked to enter the private key of the account you want to use. Remember, Ganche CLI already provides us with 10 accounts with 100 free ethers. Well, select any private key from those 10 accounts and paste it here. 

That’s it now you are all set to initiate the development process since your account is already set. 

Finally, Initiate The FRONT-END WITH REACT 

Now, since you have already covered the difficult part, its time to simply initiate the front-end part. 

Follow these setps: 

Move to the directory where you unboxed the truffle react.


• Enter the command truffle compile. 

• Then enter the command truffle migrate. 

Note: As soon as you migrate your smart contract, a small amount of ether will be deducted due to gas. Therefore, click on the Metamask extension on your browser and check if some amount has been deducted. If yes, your setup is completely fine and you are good to go. 

4. Go to the client directory and enter the command npm start. 

5. Open browser and go to localhost:3000. 

You might see a Metamask pop-up 

Note: Do you see the line that says, The stored value is: 5. The value 5 here is coming from the smart contract thus symbolizing that your front-end is in sync with your contract. 

That’s it. You have successfully integrated React with your Solidity smart contract with WEB3 and Ganache CLI. 

That’s it. You have successfully integrated React with your Solidity smart contract with WEB3 and Ganache CLI.
