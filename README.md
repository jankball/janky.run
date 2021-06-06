# janky.run
[http://janky.run/](http://janky.run/) is a BitcoinSV (BSV) exploration tool where you can see a list of tokens, current token prices, historical price charts for token transactions, and more!

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
