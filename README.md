# bitcoin_explorer

## Addresses:

### getBitcoinBalance

Get the current balance of bitcoin of every adress listed in the blockchain.

```ruby
let test 
//test 1
test = new AdressInformation();
console.log(await test.getBitcoinBalance( 'YOUR BITCOIN ADDRESS'));
```

### getAddressTransactions

Get a list of every transaction done on a specific address.

```ruby
let test 
//test 2
test = new AdressInformation();
console.log(await test.getAdressTransactions( 'YOUR BITCOIN ADDRESS'));
```

## Blocks

### getBlockInformation

Get all the information of a block in the blockchain. You get the BlockHash, the Hash of the previous and the next block, the block size and a lot of other informations.

```ruby
let test 
//test 3
test = new BlockInformation();
console.log(await test.getBlockInformation('NUMBER OF THE BLOCK'));
```

The number of the block can also be 'latest'

### get BlockList

Get a list of all the blocks mined on one day.

```ruby
let test 
//test 4
test = new BlockInformation();
console.log(await test.getBlockList('DATE'));
```

The date has to be in the following form: 15.12.2015 => '20151215'

## Transactions

### getSingleTransaction

Get the informations of a transaction with the given hashcode of the transaction.

```ruby
let test 
//test 5
test = new TransactionInformation();
console.log(await test.getSingleTransaction('HASH CODE OF THE TRANSACTION'));
```
