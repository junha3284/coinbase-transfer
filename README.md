# coinbase-transfer
This utility helps to transfer balance from my Coinbase account to my friend's on a regular basis.


## Overview

My friend and I were together to build a mining rig to mine Ethereum in 2017. We put up half of the money each person so the return should be distributed evenly as well!

At the time we were mining, we use the same program, the same pool and the same wallet. How can we distribute mined coins? This is the reason I am writing this script. 

The script runs everyday on my local machine and check Coinbase transactions to see if any mining rewards have been credited to my account in last 24 hours. If mined coins are detected, the script will send half of that amount to my friend's Coinbase account. Since Coinbase-to-Coinbase transactions are free (I guess Coinbase will just update its database to reflect the change and the transaction won't go through the blockchain at all), we find it pretty neat to have such a script!

## How to use

Run ```npm start``` which indeed it is running ```node index.js``` behind the scene.
