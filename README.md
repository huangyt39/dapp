"# dapp" 

test command in cmd 

```
truffle compile
truffle networks --clean
truffle migrate --network ganache
truffle console --network ganache

Trades.deployed().then(function(contract) {contract.createTrade("testTitle","testDetail",{value: web3.toWei('10', 'ether'), from: web3.eth.accounts[3]}).then(function(result){console.log(result)})})
Trades.deployed().then(function(contract) {contract.acceptTrade(4,{from: web3.eth.accounts[2]})})
Trades.deployed().then(function(contract) {contract.finishTrade(4,"testInfo",{from: web3.eth.accounts[2]})})
Trades.deployed().then(function(contract) {contract.finishTrade(4,"comfirmInfo",{from: web3.eth.accounts[1]})})
Trades.deployed().then(function(contract) {contract.showCount({from: web3.eth.accounts[1]}).then(function(result){console.log(result)})})
```