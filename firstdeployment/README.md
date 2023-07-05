# How this Deployment was created

This tutorial was followed: https://www.web3.university/tracks/create-a-smart-contract/deploy-your-first-smart-contract

we used sample Hello World smart contract from the Ethereum Foundation 

npm init # (or npm init --yes)

npm install --save-dev hardhat

npx hardhat - creates a new hardhat project

Select “create an empty hardhat.config.js”:

mkdir contracts
mkdir scripts

npm install dotenv --save

plugin for ether.js   https://hardhat.org/hardhat-runner/plugins/nomicfoundation-hardhat-ethers

npm install --save-dev @nomiclabs/hardhat-ethers "ethers@^5.0.0"


compile contract 

npx hardhat compile

npx hardhat run scripts/deploy.js --network goerli
Contract deployed to address: 0x170D920AD1A97816Af33eFFAa8b27D93F152D118


our contract was deployed to https://sepolia.etherscan.io/address/0x170D920AD1A97816Af33eFFAa8b27D93F152D118

npx hardhat run scripts/interact.js

npm install --save-dev @nomiclabs/hardhat-etherscan

npx hardhat verify --network goerli DEPLOYED_CONTRACT_ADDRESS "Hello World!"



