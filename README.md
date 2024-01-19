
## directory structure

```txt
.
├── Plugins
│   ├── Fake Deposit  
│   │    ├── fake_deposit_addr_list   
│   │    ├── fake_deposit_addr_opensource_list    
│   │    ├── fake_deposit_addr_opensource_unique_addr    
│   │    └── fake_deposit_hash_list  
│   ├── Fake Notification
│   │    ├── fake_notification_addr 
│   │    └── fake_notification_opensource_addr   
│   ├── Inconsistent transferFrom().xls
│   ├── Salmonella
│   │    ├── Salmonella contracts in Goerli
│   │    └── Salmonella contracts in Mainnet
│   └── Unauthorized Token Burning.xlsx
├── CRYPTO-SCOUT
│   ├── All
│   │    ├── erc_result 
│   │    ├── pattern_result 
│   │    ├── handle_intra-contract 
│   │    └── irrelevant_variables  
│   ├── Open_source
│   │    ├── erc_result
│   │    ├── pattern_result 
│   │    ├── fake_notification_addr 
│   │    ├── handle_intra-contract 
│   │    └── irrelevant_variables 
│   ├── source_code    
│   ├── token_bytecode     
│   └── unique_bytecode
```

## Description
* `Plugins`:results of five plugins
 * `Fake Deposit`:tokens with fake Deposit
    - `fake_deposit_addr_list`：all addresses that are not unique
    - `fake_deposit_addr_opensource_list`：all open source addresses that are not unique
    - `fake_deposit_addr_opensource_unique`：all open source addresses that are unique
    - `fake_deposit_hash_list`：hash list of unique
 * `Fake Notification`: tokens with fake notifications
    - `fake_notification_addr `：all addresses of tokens with fake notifications
    - `fake_notification_opensource_addr`：opensource addresses of tokens with fake notifications
 * `Inconsistent transferFrom().xlsx `：the result of plugin Inconsistent transferFrom()
 * `Salmonella`: Salmonella contracts
    - `Salmonella contracts in Goerli`：all addresses of Salmonella contracts in Goerli
    - `Salmonella contracts in Mainnet`：all addresses of Salmonella contracts in Mainnet
 * `Unauthorized Token Burning.xlsx`：the result of plugin Unauthorized Token Burning
* `CRYPTO-SCOUT`:data collected and processed
 * `All`:token data
  * `erc_result`: tokens with different token standard
    - `*_sol` tokens written by solidity;
    - `*_vy` tokens wrriten by vyper.
  * `pattern_result`: tokens of 10 patterns.
  * `handle_intra-contract`: executing each intra-contract function invocation only once, these tokens will be missed.
  * `irrelevant_variables`: contracts with irrelevant variables
 * `Open_source`:open source parts of the data in All
 * `source_code`: source code of contracts.
 * `token_bytecode`: runtime bytecode of token contracts.
 * `unique_bytecode`: unique runtime bytecodes.
