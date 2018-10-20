# Coinbase-Transfer
Coinbase-Transfer transfers balance from one [Coinbase](https://www.coinbase.com/) account to another on a regular basis.


## Motivation

My friend and I were together to build a mining rig for Ethereum in 2017. We put up half of the money each person so the return should be distributed evenly as well!

At the time we were mining, we use the same program, the same pool and the same wallet. How can we distribute mined coins? This is the reason I am writing this script. 

The script runs everyday on my local machine and check Coinbase transactions to see if any mining rewards have been credited to my account in last 24 hours. If mined coins are detected, the script will send half of that amount to my friend's Coinbase account. Since Coinbase-to-Coinbase transactions are free (I guess Coinbase will just update its database to reflect the change and the transaction won't go through the blockchain at all), we find it pretty neat to have such a script!

## How to use

1. Create a file named ```config.js``` by copying all the contents in ```config.sample.js```. Replace the config settings in ```config.js``` with yours. Instructions and meanings for each config setting are available inside ```config.sample.js```. 
2. Run ```npm start``` to trigger ```node index.js``` behind the scene.
