# janky.run
[http://janky.run/](http://janky.run/) is a BitcoinSV (BSV) exploration tool where you can see a list of tokens, current token prices, historical price charts for token transactions, and more!

## What you can do at janky.run

* Get a list of all of the tokens that have been created
* Get a list of all of the creators of those tokens and see which other tokens they have created
* Get prices for tokens in satoshis or US dollars
* Get price charts for tokens in US dollars
  * Generating a price chart requires that we have more than a couple transactions for the token - enough to generate a nice looking chart.
  * I have discovered not all tokens have enough transactions, in which case I can still show the price, but not a chart.

## Technologies and Data Used

The application includes:

* API: Flask + python
* UI: React + Material UI
* Run DB data crawler: python

The API stack includes:

* Docker containers
* nginx web server and proxy
* MongoDB data storage
* Redis caching layer

Data sources include:
* [RUN-DB](https://github.com/runonbitcoin/run-db) with modifications
* [CoinGecko for BSV prices](https://www.coingecko.com/en)
