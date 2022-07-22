# 19-challenge
 Fintech Finder is an application that its customers can use to find fintech professionals from among a list of candidates, hire them, and pay them


## Technology
import os
import requests
from dotenv import load_dotenv
load_dotenv()
from bip44 import Wallet
from web3 import Account
from web3 import middleware
from web3.gas_strategies.time_based import medium_gas_price_strategy


## Installation Guide
Using the Conda package manager: [My GitHub Project](https://github.com/ALovettII/19-challenge.git)

pip install web3==5.17
To install the ethereum-tester library, check that your dev environment is active, and then run the following:
pip install eth-tester==0.5.0b3
To install the mnemonic package, check that your dev environment is active, and then run the following:
pip install mnemonic
To install the bip44 package, check that your dev environment is active, and then run the following:
pip install bip44


## Usage
1. `finiech_finder.py`
    * It contains the code associated with the web interface of your application
    * Write all of your code for this Challenge in this file.
2. `crypto_wallet.py`
    * Contains the Ethereum transaction functions that you have created throughout this module’s lessons
    * Using import statements:
        * You will integrate the crypto_wallet.py Python script into the Fintech Finder interface program (found in the fintech_finder.py file)

*To confirm that you have successfully created the transaction:
    * You will save screenshots to the README.md file of your GitHub repository for this Challenge assignment.*

Use Cases:
* Generate a new Ethereum account instance by using the mnemonic seed phrase provided by Ganache.
* Fetch and display the account balance associated with your Ethereum account address.
* Calculate the total value of an Ethereum transaction, including the gas estimate, that pays a Fintech Finder candidate for their work.
* Digitally sign a transaction that pays a Fintech Finder candidate, and send this transaction to the Ganache blockchain.
* Review the transaction hash code associated with the validated blockchain transaction.


Sections:
1. Import Ethereum Transaction Functions into the Fintech Finder Application
2. Sign and Execute a Payment Transaction
3. Inspect the Transaction on Ganache


MNEMONIC = 'YOUR MNEMONIC SEED PHRASE HERE'


## Contributors
Created by Arthur Lovett
