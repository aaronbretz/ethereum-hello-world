# ethereum-hello-world

## What you'll need

1) [Mist](https://github.com/ethereum/mist/releases). Note, it will take some time and give our take 8GB of memory to sync your full ethereum node to the test-net.
2) [Node.js](https://nodejs.org/en/download/)
3) [MetaMask](https://metamask.io/)

## Instructions

After you have installed all the requirements and cloned this repo,

1) Ensure you are running on the test-net by going to Develop->Network. DO NOT DO ANY WORK ON MAIN NETWORK. Doing so will only cost you lots of expensive ether.
2) Next,create an account for yourself going to Accounts->New Account.
3) Find yourself some ether. You can mine some by going Develop->Start mining (this should take about 1-2 hours to mine a block). You can try on of the test ether [faucets](http://faucet.ropsten.be:3001/). Or lastly, ping Aaron for some.
4) Copy the contents of the contract named ERC20.sol 
5) Go to your ethereum wallet and click contracts in the top right corner, then click add new contract and replace the default contract with our contract by pasting into the editor.
6) To the right of the editor, click the dropdown to select BPThreewards to deploy.
7) Scroll to the bottom and click deploy contract.
8) After the contract has been verified, it should show up in your wallet. Once it shows up in the contracts area of your wallet, click on it, which will bring you to the admin page.
9) Locate the Copy Interface button and copy the ABI.
10) Open the app.js file located in the public/javascripts directory.
11) Paste the ABI on line 17.
12) Copy the contract address and paste it into line 19 of app.js
13) Open a terminal and navigate to the folder where this repo was cloned.

`node server`

14) Open the [app](https://localhost:3000)
15) Import the account you created into your MetaMask plugin

Import the key with a json file. Navigate to the home directory by pressing cmd+shift+h, then go Library->Ethereum->testnet->keystore and import the files for the account you want to access in your browser.

16) Refresh the page and if you are using the account you deployed the contract with, you should see the balance reflected in the top right corner.
17) You should now be able to interact with your newly created smart contract. GO NUTS!
