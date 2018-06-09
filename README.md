# Arionum Scripts

A series of useful scripts for managing an Arionum testnet and/or mainnet node.  
For more information see http://www.arionum.com

# SCRIPT: Arionum Node Setup 

This script will install and configure Nginx, PHP-FPM 7.2, and MariaDB(Mysql).  
It will clone the Arionum node software from https://github.com/arionum/node and configure the system.  

## Arionum Node Requirements
1. Ubuntu 16.04 (may work on other debian/ubuntu distros)  
2. Fresh clean vanilla server.  
3. Nginx, PHP-FPM 7.2, and MariaDB will be installed and configured.  
4. Not responsible if you hose your existing setup

## Arionum Node Installation 
`$ cd ~`  
`$ wget https://github.com/KyleFromOhio/arionum-scripts/blob/master/arionumNodeSetup.sh`  
`$ chmod +x arionumNodeSetup.sh`

## Arionum Node Usage
`$ sudo bash arionumNodeSetup.sh mainnet install`

## Additional Options
`$ sudo bash arionumNodeSetup.sh mainnet <install|upgrade|rebuild|reset>`  
`$ sudo bash arionumNodeSetup.sh testnet <install|upgrade|reset>`  
 
 install   -- install Arionum node and required software and configure system  
 upgrade   -- upgrade existing Arionum node system and codebase  
 rebuild   -- will empty database and restore to latest snapshot  
 reset     -- will empty database and trigger db update  

