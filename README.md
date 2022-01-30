# Stock Analyzer
Stock Analyzer application which helps you analyze and track your stocks and cryptos in a single place.

**Business Case**
A lot of people starting working from home due to Covid since 2020. This led to a lot of them to start investing actively in stocks and cryptos. I also got up in that bandwagon and soon started to actively trade in stocks, etf's and cryptocurrencies. This also led me to research and start signing up for popular stock advisor websites like Motley fool, Near futures, IPO Scoop, etc. During the first six plus months it was easy as I had a small portfolio of few stocks and a single broker, but soon by the close end of 2020 my portfolio began to increase to 100+ stocks and by this time I had begun to actively trade with multiple brokers like TD Ameritrade, Vanguard, Robinhood, Crypto.com, Coinbase, etc.

It soon became a nightmare to me to keep track of what I have invested and how much I have invested in a stock. I began to manually maintain it using TD Ameritade using the watchlist, but it also had limitations and neede constant sync up's between my other accounts. TD also did not support Cryptos which had become so popular and it started really picking off.

To handle this, I started off with the new idea of creating a Stock Analyzer application, which helped me 
a) Aggregate all my positions across various accounts
b) Check my investment's on each stock/crypto across all accounts
c) Classify my investment based on advisory (Mothley, Near Futures, IPO Scoop, etc
d) Get realtime picture of my investment's by integrating with Yahoo Finance, Coin Market api's by getting realtime prices
e) Analyze the Day% gain/loss to determine if its the best time to buy or sell based on advisory analysis
f) Analyze the profitability for each of these advisories thus driving the investment up/down based on returns

I have constantly been adding functionalities to this application which currently is in it's 10th version of existence. I am happy and always have this running and never have to login to my other trading accounts, except when it's time to trade. 

I have already shared this with 2 of my close friends who use this on a regular basis and advise on additional functionality which helps me improve it.


**Technical Information**
This project is entirely written in React 17 & Java 11. The backend used is H2 database.


**Future Plans**
I plan to have this hosted on AWS infrastructure in the near term, so I can even make it available for a wider audience. I intend to keep it free initially and then start to make it available as a paid version in the future. There will definitley be a lot of changes needed to make it available on AWS and support multiple users'.
Below are some of to do list to achieve this
1) RDS - Oracle / Aurora / Postgres - Workaround to see if free H2 can support 50-100 users w/o performance impacts
2) Support user logins
3) Modify tables to store user specific data
4) Instrument table can be shared but some key information has to stripped out
5) Dynamic support of additional Advisories as adding new should NOT result in adding columns to table
6) Dynamic UI to support additional Advisories OR have at least placeholder's to support User's
7) Backup's & restores of Core database tables in case of any issues/corruption
8) Support Blue/Green deployment for new versions
9) Support User Types(future) in case of some specific paid features
