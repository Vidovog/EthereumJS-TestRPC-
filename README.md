# EthereumJS-TestRPC-
Simple JavaScript Smart Contract Interaction with EthereumJS-TestRPC:
const Web3 = require('web3');
const web3 = new Web3(new Web3.providers.HttpProvider('http://localhost:8545'));

const abi = [...]; // Your smart contract ABI
const contractAddress = '0x123456789abcdef123456789abcdef123456789a';
const contract = new web3.eth.Contract(abi, contractAddress);

// Example: Calling a smart contract method
contract.methods.myMethod().call().then(console.log);
