# brownie_fund_me
Smart Contract Application

FundMe
FundMe is a decentralized application that allows users to fund projects in Ethereum (ETH) cryptocurrency. This smart contract utilizes the Chainlink oracle to fetch the latest price data for ETH and convert it to USD.

Installation
Clone or download the repository.
Install the required dependencies using pip install.
Compile the Solidity contract using brownie compile.
Deploy the contract to the Ethereum network using brownie run scripts/deploy.js --network <network-name>.
Usage
To use the FundMe smart contract, you can call the following functions:

fund(): Allows a user to fund a project by sending ETH to the contract. The amount must be at least 50 USD worth of ETH, according to the current ETH/USD price provided by the Chainlink oracle.
getEntranceFee(): Returns the minimum entrance fee required to fund a project, based on the current ETH/USD price.
getVersion(): Returns the version of the Chainlink oracle used by the contract.
getPrice(): Returns the latest ETH/USD price from the Chainlink oracle.
getConversionRate(uint256 ethAmount): Returns the equivalent USD value of the given ETH amount, based on the current ETH/USD price.

