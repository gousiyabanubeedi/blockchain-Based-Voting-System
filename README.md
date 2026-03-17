# Blockchain-Based Voting System

A decentralized voting application built using blockchain technology to provide secure and transparent elections.

## Project Overview

This project demonstrates how blockchain can be used to build a secure digital voting system.  
Votes are stored on the blockchain using smart contracts, ensuring transparency and preventing duplicate voting.

## Features

- Secure blockchain-based voting
- Smart contract vote validation
- Prevention of duplicate voting
- Transparent vote counting
- Admin panel to manage candidates

## Technologies Used

- Node.js
- SmartContracts
- Truffle Framework
- Ganache
- MetaMask
- Mysql
- Python
- Web technologies

## Project Structure
dVoting                                                                                                                                                                                                            
├── client                                                                                                                                                                                                    
├── contracts                                                                                
├── migrations                                                                                                                                                                                    
├── truffle-config.js                                                                                                                                                                                         
└── README.md

## How the System Works

1. Admin creates the election and adds candidates.
2. Users log in to the system.
3. Voters select a candidate and cast their vote.
4. The vote is recorded on the blockchain through a smart contract.
5. The system ensures each user can vote only once.
6. Results are calculated automatically.

## Instruction to run 
1.Open a terminal.

2.Clone the repository by using the command
git clone https://github.com/
Download and install Ganache.

3.Create a workspace named developement, in the truffle projects section add truffle-config.js by clicking ADD PROJECT button.

4.Download Metamask extension for the browser.

5.Now create wallet (if you don't have one), then import accounts from ganache.

6.Add network to the metamask. ( Network name - Localhost 7575, RPC URl - http://localhost:7545, Chain ID - 1337, Currency symbol - ETH)

7.Open MySQL and create database named voter_db. (DON'T USE XAMPP)

8.In the database created, create new table named voters in the given format and add some values.
9.Install truffle globally
10.npm install -g truffle
11.Go to the root directory of repo and install node modules
12.npm install
13.Install python dependencies
14.pip install fastapi mysql-connector-python pydantic python-dotenv uvicorn uvicorn[standard] PyJWT
Usage
Note: Update the database credentials in the ./Database_API/.env file.
Open terminal at the project directory

15.Open Ganache and it's development workspace.
16.open terminal in project's root directory and run the command

16.truffle console - then compile the smart contracts with command
17.compile - exit the truffle console

18.Bundle app.js with browserify

19.browserify ./src/js/app.js -o ./src/dist/app.bundle.js
Start the node server server

20.node index.js
Navigate to Database_API folder in another terminal

21.cd Database_API
then start the database server by following command

22.uvicorn main:app --reload --host 127.0.0.1
In a new terminal migrate the truffle contract to local blockchain
23.truffle migrate

## Learning Outcome
Through this project, I gained practical understanding of:
- How blockchain can be used for secure voting systems
- Basic smart contract development using Solidity
- Deploying contracts using Truffle and Ganache
- Connecting a web application


