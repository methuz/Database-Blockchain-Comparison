# Database & Blockchain Comparison

| Service | Example | Distributed | Keep Value | Node Consensus | Atomicity | Consistency | Isolation | Durability | Persistency | Integrity | P2P | Trustless | Public Access | Programable | Can  Keep Large Data | Note |
|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|  
| Service Discovery | ETCD, Zookeeper | T | F | T | F | F | F | F | F | T | T | F | F | F | F | Lite distributed database with built-in consensus |
| Traditional/Modern Database | MongoDB, MySQL, Hadoop | Depends | F | Depends | Depends | Depends | Depends | T | T | Depends | Depends | F | F | Depends | T | Most problem solved with them |
| In-memory Database | Redis, Memcache | F | F | F | Depends | T | F | Depends | F | F | F | F | F | F | F | fast/lite temporary database |
| Traditional P2P File Sharing | Bittornt | T | F | F | Undefined** | Undefined** | Undefined** | Undefined** | T | T | T | T | Partial*** | F | T | No transaction/update |
| Version Control System | Git/Git Servers | Partial | F | F | T | Depends | F | T | T | Partial | Partial | F | Depends | Partial | Partial | Depends on Configuration and plugins |
| Traditional Cryptocurrency | Bitcoin | T | T | T | T | T | T | T | T | T | T | T | T | Partial | F | Bitcoin can be programed? Yeah Bitcoin Script |
| Decentralized Application Platform/Crypto 2.0| ETH/EOS and/or etc. | T | T | T | T | T | T | T | T | T | T | T | T | T | F | "Jack of all trade, Master of none" |
| Trust based Cryptocurrency | Stellar | T | T | T | T | T | T | T | T | T | T | F | T | Partial | F | Blockchain + Federation Server |
| Trust-based Distributed Application | Matrix Chat | T | F | F | Undefined** | Undefined** | Undefined** | Undefined** | T | Partial | T | F | T | T | T | Identity Server + Federation Server |
| P2P File System | IPFS | T | F | F | Undefined** | Undefined** | Undefined** | Undefined** | T | T | T | T | Partial*** | F | T | Bittorent with hashed url |
| Private DLT | Hyperledger | T | F | T | T | T | Depends | T | T | T | T | F | F | T | F | You need to know more about security than blockchain to use it |

** Undefined since there is no transaction or updating function
*** Partial depends on how file host let people to discover

## What are all these mean? (in TLDR form)
### Distributed
Data can be distributed (replicated) across multiple node

### Keep Value
It can contains value in economic sense.

### Node Consensus
There is a mechanism that allow all node to agree upon some fact, such as Who is the leader of the cluster? What's the latest state of the data.

### Atomicity
Half done transaction shall not possible.

### Consistency
No illegal (In Computer Science sense) transaction can be stored. But it does not mean the data is logically correct (in application sense)

### Isolation
If there are more than one transaction submitted at the same time, Service shall treat them as one after another.

### Durability
Transaction must be written on harddisk to prevent stored data from missing.

### Persistency
Similar to durability but not only limited to transaction, Data must not be erased unless it is really meant to be deleted.

### Integrity
All node always contains and return the same data.

### P2P
Node talk to another node on their own, No master needed.

### Trustless
Need trust to interact, share data with.

### Public Access
Anyone in the world can look at the data

### Programable
Turing complete = T

### Note
My comment
