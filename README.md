# MC Week 4 Project
**Setting Up the Arbitrum Sepolia Testnet Environment**

I opened MetaMask and click on the network dropdown, first it was on Arbitrum one and I scroll down to select Add Network button.
I clicked on Add a network manually and filled the Network Name, New RPC URL, Chain ID, Currency Symbol and Block Explorer URL, then I clicked on save. I
went back to my Network and changed it to Arbitrum Sepolia.

**Acquire Testnet ETH**

I went to Chainlink Faucet through https://faucets.chain.link/sepolia (Arbitrum Sepolia Drip 0.1ETH was already selected) so I clicked continue and connected my MetaMask wallet 
to the Chainlink Faucet and clicked on Get Tokens. I switched my network to Arbitrum Sepolia to check my balance but it was still 0ETH. I went to networks and under show 
test networks I clicked on Sepolia and 
there was 0.1Sepolia ETH. I went to Arbitrum Bridge through https://bridge.arbitrum.io/, connected my MetaMask wallet. On the bridge, I selected Arbitrum Sepolia as the destination.
On the amount, I entered 0.1 and comfirmed the transaction.  The transfer was complete and my balance also appeared on my MetaMask wallet.

**Write a Smart Contract in Remix**

I opened Remix IDE https://remix.ethereum.org/ and on the File Explorer I created a new workspace and named it "Arbitrum_deployment". Under it, I created a new file 
and named it "HelloArbitrum.sol".
I wrote a smart contract "HelloArbitrum" to store a message. I added a constructor to set the initial message when the contract is deployed. I created an updateMessage function to allow 
anyone to change the message stored in the contract(this was made public).

**Compile and Deploy the Contract**

I clicked on the “Solidity Compiler” tab (left sidebar, the third icon after the search icon), I ensured that the compiler version was 0.8.25 and I 
clicked the Compile HelloArbitrum.sol button.
On “Deploy & Run Transactions” tab, under Environment, I selected “Injected Provider – MetaMask.” and I was asked to approve connection so I clicked Connect.
In the Deploy & Run Transactions tab, I selected HelloArbitrum from the dropdown under Contract. In the input box, I typed "Hello, Arbitrum" and clicked the Deploy button.

**Interact with the Contract**

I clicked the message() function to view the initial message and "Hello, Arbitrum" was written. In the updateMessage() function’s input box, I typed "Welcome to Layer 2"
and clicked the updateMessage() button and confirm the transaction in MetaMask. The transaction was confirmed, click message() again to see the updated message.
In Remix, I copied the address of the deployed contract and went to Arbiscan https://sepolia-explorer.arbitrum.io/ and pasted the
contract address in the search bar, the details of the deployment and interactions were shown.
