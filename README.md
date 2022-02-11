# Financial Planning Tools

## Table of Contents:

* Create a Financial Planner for Emergencies
* Evaluate the Emergency Fund
* Create a Financial Planner for Retirement

### Create a Financial Planner for Emergencies


* Step 1: Review Endpoint URLs for the API Calls to Free Crypto API**

`btc_url = 'https://api.alternative.me/v2/ticker/Bitcoin/?convert=USD'
eth_url = 'https://api.alternative.me/v2/ticker/Ethereum/?convert=USD`

api_key = os.getenv('ALPACA_API_KEY')`


* Step 2: Use request library to get the current price of BTC and ETH:

`btc_response = requests.get(btc_url).json()`

`btc_price = btc_response['data']['1']['quotes']['USD']['price']`

* Step 3: Calculate the value of BTC and ETH in the portfolio:

`btc_value = btc_coins * btc_price`

