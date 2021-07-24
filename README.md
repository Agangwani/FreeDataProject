# FreeDataProject
This is the official repository for the FreeDataProject. 

Disclaimer: 

Please do keep the spirit of open source alive here. Everyone is welcome to pull from the main branch or any sub-branches I create but please do push to a separate branch that is aptly named so there's no confusion. 

The way we wanted to run this project was as an idea that's slowly built into a reality. More details will be added as we continue to workshop. The idea here is that everyone who wants to learn new technologies alongside us are welcome to do so with this idea as a general framework. Feel free to change or add whatever you'd like. Just sign it with your name and the date so we know where changes are made. 

Again, I want to stress that right now it's an infant of an idea. So far I've experimented with some libraries to scrape data off local devices as a means of data gathering. Continuing forward, an example of a path you can take is to implement a basic localized blockchain system with arbitrary data. Then we can store the data on that blockchain or work towards that. Or you can look at a distributed database system which is essentially going to be our distributed ledger through blockchain, and you learn how to aggregate/work with data there which should lead to insights on how our smart contracts will work. 

Prerequisite: 

For the longest time, we have been content with signing away our data to large companies who trade it at will; generating user profiles for targeted advertisements. However, I've long questioned this system. Perhaps, at one time, google and other search engines were considered a luxury to be able to use. However, they've become a necessary utility in todays societies. If companies are investing millions of dollars into researching how to make applications more addictive to force us to spend more time using them, we should be able to profit at least partially through this system, one that takes up so much of our time every day. 


Intent: 

The intent of this project is to create a decentralized application that will allow users to actively track and sell their own data. There are a few layers to a potential design which will be outlined below.


Approach One: Decentralized Application 

Layer One: Blockchain

Blockchains are nothing but decentralized databases with dynamic transactions. Our blockchain layer will be used to store the data that users actively generate. That is where Ethereum or perhaps another alternative come into play. We utilize the ethereum blockchain to store data that we have collected. We could alternatively build a separate fork of ethereum so it's ecosystem is not tied down with ethereums. The idea is that our blocks are going to be collections of data such as website url, and time to begin with. We can add more comprehensive data collection systems; however, this is a good start. 

We have established that our blockchain is going to store user data such as websites visited. In order to maximize data utility for the end users i.e. the companies that are buying it, we may want to bundle data together. Thus we can create a system that, every perhaps 1 hour, it pushes a new block to the blockchain which contains all of the relevant user data from the last hour. Next, independent miners will "mine" the block and approve it for the blockchain. They will be paid a certain fee for doing this. 

Now we have some framework for how blocks are going to be added, what they will contain, and some approval system. This is a good enough framework for now and we can move on to the next layer 

Layer Two: Smart Contracts

Smart contracts are a concept specific (I believe) to ethereum and it's general purpose nature. Smart contracts are described as "vending machines". The conceptual idea of this layer is that companies will interact with these smart contracts to request data from the blockchain. The data generated can perhaps be random, or have some kind of searching factor involved. Either way, the specifics can be sorted out later; but the general purpose of the smart contract is going to be as a middle man to interact with the blockchain. 

Example: Company A requests data from individuals in this demographic. The data is read from the blockchain into the smart contract and stored in escrow. Once funds from Company A have been deposited, they can utilize an API to request the data. This is where some security measures will have to be built in so not everyone can view the data without paying; especially because blockchains are inherently open for viewing. An example solution could be to encrypt the data when it's stored on the blockchain. 

Thus companies now, with smart contracts, have some mechanism of buying data directly from the users. The smart contracts will have to be written such that they are generalized and funds are deposited appropriately into each users account. Once funds are verified, the data is released and available for viewing. Because we generate so much data every day, there won't be anything close to a shortage and another option for monetiziation (throwing it out there) is to allow for companies to actively stream data from the blockchain for an enhanced fee. 

NOTE: 
The blockchains "ecosystem" is supported by companies buying some "token" to pay for the data. Thus when miners approve the data transactions, they are awarded something of monetary value so long as companies buy data. Therefore, as the network becomes more valuable and companies buy from it more, the token is also grown in value. 



Layer 3: Etherum nodes for execution of smart contracts

This one is pretty simple. If we wanted to launch onto the ETH network, we will have to use eth nodes to actually execute the smart contracts

Approach Two: Semi Centralized Application
