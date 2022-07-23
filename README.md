# 19-challenge
 Fintech Finder is an application that its customers can use to find fintech professionals from among a list of candidates, hire them, and pay them


## Technology
This project uses the following libraries:
* [Web3.py](https://web3py.readthedocs.io/en/stable/overview.html)
* [ethereum-tester](https://pypi.org/project/ethereum-tester/0.1.0a4/)
* [mnemonic](https://pypi.org/project/mnemonic/)
* [bip44](https://pypi.org/project/bip44/)
* [Ganache](https://www.trufflesuite.com/ganache)


## Installation Guide
Using the Conda package manager: [My GitHub Project](https://github.com/ALovettII/19-challenge.git)

While your dev enviroment is active, run the following in your terminal: 
```shell
# To install the Web3.py librar
pip install web3==5.17

# To install the ethereum-tester library
pip install eth-tester==0.5.0b3

# To install the mnemonic package
pip install mnemonic

# To install the bip44 package
pip install bip44
```


## Usage
### Main Sections:
1. Import Ethereum Transaction Functions into the Fintech Finder Application
2. Sign and Execute a Payment Transaction
3. Inspect the Transaction on Ganache

### File Descriptions:
1. `fintech_finder.py`
    * It contains the code associated with the web interface of your application
2. `crypto_wallet.py`
    * Contains the Ethereum transaction functions that you have created throughout this module’s lessons

### Use Cases:
* Generate a new Ethereum account instance by using the mnemonic seed phrase provided by Ganache.
* Fetch and display the account balance associated with your Ethereum account address.
* Calculate the total value of an Ethereum transaction, including the gas estimate, that pays a Fintech Finder candidate for their work.
* Digitally sign a transaction that pays a Fintech Finder candidate, and send this transaction to the Ganache blockchain.
* Review the transaction hash code associated with the validated blockchain transaction.

### Deployment:
For successful deployment, you will need to create a `.env` file with your mnemonic from Ganashe:
```python
MNEMONIC = 'YOUR MNEMONIC SEED PHRASE HERE'
```

To launch the Streamlit application from your terminal:
1. Navigate to the project folder that contains your .env file and the fintech_finder.py and crypto_wallet.py files.
2. Activate your Conda dev environment
3. Run:
    `streamlit run fintech_finder.py`


### Screenshots: Transaction Verification
#### Fintech Finder Application (with transaction hash
Verify the transaction using the resulting hash and the account addresses of each party:
![Fintech Finder](https://github.com/ALovettII/19-challenge/blob/main/Images/ss_app.png)

#### Transaction Details
On Ganache: Verify completion by matching the transaction hash:
![Transaction](https://github.com/ALovettII/19-challenge/blob/main/Images/ss_transaction.png)

#### Client Balance
We can see that the client's (your) balance (100 inital ether) has decreased equal to the amount of the transaction (8 ether).
![Client Balance](https://github.com/ALovettII/19-challenge/blob/main/Images/ss_balance.png)

#### Block 1
Ganashe also displays the data contained in our Block 1:
![Block 1](https://github.com/ALovettII/19-challenge/blob/main/Images/ss_block.png)


## Contributors
Created by Arthur Lovett
