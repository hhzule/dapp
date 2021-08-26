npx create-react-app my-app --template typescript -frontend

truffle init -backend
touch backend/contracts/Marketplace.sol- add code
change truffle config
  contracts_directory: './contracts/',
  contracts_build_directory: '../frontend/src/abis/',
truffle compile
 deploy the mart contract to our Ganache 
 touch migrations/2_deploy_contracts.js
 This file tells Truffle to to deploy our smart contract to the blockchain. It's kind of like a migration file for a traditional database if you're familiar with that. Also, note that the migration files are numbered so that Truffle knows which order to run them in.
 truffle migrate --reset
 smart contract tests 
 $ mkdir test
$ touch test/Marketplace.test.js
passed, 
add function- create product and variables to contract
test again
add tools to our test suite 

require('chai')
.use(require('chai-as-promised'))
.should()

write tests
and test
npm i     "chai": "^4.3.4",
    "chai-as-promised": "^7.1.1",

add function- sell product and variables to contract
add test
truffle migrate --reset
done

frontend
mkdir frontend
npx create-react-app
npm i web3
Connect Metamask to our Ganache personal blockchain instance
import Web3 from 'web3'
instantiates web3.
