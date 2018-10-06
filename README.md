# Database & Blockchain Comparison

| Service | Example | Distributed | Keep Value | Node Consensus | Atomicity | Consistency | Isolation | Durability | Persistency | Integrity | P2P | Trustless | Public Access | Programable | Can  Keep Large Data | Note |
|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|-----|  
| Service Discovery | ETCD, Zookeeper | T | F | T | F | F | F | F | F | T | T | F | F | F | F | Lite distributed database with built-in consensus |
| Traditional/Modern Database | MongoDB, MySQL, Hadoop | Depends | F | Depends | Depends | Depends | Depends | T | T | Depends | Depends | F | F | Depends | T | Most problem solved with them |
| In-memory Database | Redis, Memcache | F | F | F | Depends | T | F | Depends | F | F | F | F | F | F | F | fast/lite temporary database |
| Traditional P2P File Sharing | Bittorrent | T | F | F | Undefined** | Undefined** | Undefined** | Undefined** | T | T | T | T | Partial*** | F | T | No transaction/update |
| Version Control System | Git/Git Servers | Partial | F | F | T | Depends | F | T | T | Partial | Partial | F | Depends | Partial | Partial | Depends on Configuration and plugins |
| Traditional Cryptocurrency | Bitcoin | T | T | T | T | T | F | T | T | T | T | T | T | Partial | F | Bitcoin can be programed? Yeah Bitcoin Script |
| Decentralized Application Platform/Crypto 2.0| ETH/EOS and/or etc. | T | T | T | T | T | F | T | T | T | T | T | T | T | F | "Jack of all trade, Master of none" |
| Trust based Cryptocurrency | Stellar | T | T | T | T | T | F | T | T | T | T | F | T | Partial | F | Blockchain + Federation Server |
| Trust-based Distributed Application | Matrix Chat | T | F | F | Undefined** | Undefined** | Undefined** | Undefined** | T | Partial | T | F | T | T | T | Identity Server + Federation Server |
| P2P File System | IPFS | T | F | F | Undefined** | Undefined** | Undefined** | Undefined** | T | T | T | T | Partial*** | F | T | Bittorent with hashed url |
| Private DLT | Hyperledger | T | F | T | T | T | F | T | T | T | T | F | F | T | F | You need to know more about security than blockchain to use it |

** Undefined since there is no transaction or updating function
*** Partial depends on how file host let people to discover
