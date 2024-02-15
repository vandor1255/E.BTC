
# E.BTC Miner for Pulsechain

## What is E.BTC?

- EVMBitcoinToken is a meme coin on Pulsechain with a 21M supply.
- Initial mints (first 210,000 transactions) produced 50 eBTC rewards with a maximum of 25 transactions per wallet. 
- Every 210,000 transactions, the mint reward decreases by half.
- URL: https://www.notyourmomsbitcoin.com


## E.BTC Miner - Features

- Automatically and seamlessly generates new wallets for each mining session, thereby circumventing the limitation of 25 transactions per wallet.
- Dynamic Adjustment to Gas Prices (mints at user-specified gas limits)
- Mint E.BTC tokens based on predefined conditions (defined PLS balance or defined number of transactions)
- Transfer mined E.BTC tokens and leftover PLS back to the main wallet.
- Detailed logging of mining activities and transactions.

## Video Demo

- https://twitter.com/xenpub/status/1757975948614381868

## Requirements

- Python 3.8 or higher
- `web3` Python library
- `requests` Python library

## Installation

1. Ensure Python 3.8+ is installed on your system.
2. Install required Python libraries:
   ```bash
   pip install web3 requests
   ```

## Configuration

Before running the miner, configure the following settings in the `E.BTC-Miner.py` script:

- `main_wallet_address`: Your main Pulsechain wallet address.
- `main_wallet_address_private_key`: Private key for the above wallet.
- Gas-related settings such as `only_claim_if_gas_is_below` to specify the maximum gas price (in Gwei) you're willing to pay for transactions.
- `max_Spend_PLS`: The maximum amount of PLS you want to spend on mining.
- `max_total_transactions`: The maximum number of transactions before the program stops.
- `cooling_period_between_new_wallets`: Time in seconds to wait before creating a new wallet for mining.

**Warning:** Be cautious with your private key and never share it with others.

## Usage

To start the mining process, execute the script from the command line:

```bash
python E.BTC-Miner.py
```

The script will automatically handle the mining process based on the configured parameters, including wallet creation, token minting, and funds transfer.

## License

The open source license under which this script is released: MIT


## Follow Us:

- https://twitter.com/xenpub/


## Donate

- If we saved you time or money: https://xen.pub/donate.php


# DISCLAIMER:

You are solely responsible for ensuring the secure configuration and operation of this script, including but not limited to protecting it from unauthorized access by third parties. Failure to do so may result in the loss of your private keys, or other cryptocurrencies stored in your account. You should exercise caution and only run this script on a secure workstation or server.
By using this script, you acknowledge that you understand the inherent risks associated with running this script and that you agree to use this script at your own risk.
The creator of this script will not be held liable for any damages, loss of funds, or other negative consequences that may result from you or any third party using this script.
You are solely responsible for any actions taken using this script, and for securing your private keys and other sensitive information.
This script is provided 'as is,' and the creator makes no warranty, express or implied, of any kind.

