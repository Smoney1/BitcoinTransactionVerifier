# BitcoinTransactionVerifier

This repository contains Python functions for interacting with Bitcoin transactions and prices.

## Functions

### `verify_transactions`

This function queries and verifies Bitcoin transactions for a given address within a specified time period.

#### Parameters
- `address` (str): The Bitcoin address to check for transactions.
- `period_hours` (int, optional): The time period in hours to look back for transactions. Default is 24 hours.

#### Returns
- `float`: The total amount of Bitcoin received by the address in the specified period.

#### Example
```python
total_received = verify_transactions('your_bitcoin_address')
print(f"Total received in the last 24 hours: {total_received} BTC")
```

### `get_bitcoin_price`

This function fetches the current price of Bitcoin in USD from the CoinGecko API.

#### Returns
- `float`: The current price of Bitcoin in USD.

#### Example
```python
btc_price = get_bitcoin_price()
if btc_price:
    print(f"Current Bitcoin price: ${btc_price} USD")
```

## Installation

To use these functions, you need to have Python installed on your system along with the `requests` library.

```bash
pip install requests
```

## Usage

After installing the required library, you can import and use these functions in your Python scripts.

## Contributions

Contributions are welcome. Please feel free to submit a pull request or open an issue.

## License

This project is licensed under the MIT License - see the LICENSE file for details.
