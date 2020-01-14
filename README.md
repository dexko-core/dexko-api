DEXKO API
===================



API List
-------------
<table>
  <tr><th>URL</th><th>Description</th></tr>
  <tr><td>https://api.dexko.co.kr/v2/public/market/all</td><td>Market</td></tr>
  <tr><td>https://api.dexko.co.kr/v2/public/ticker</td><td>Ticker</td></tr>
  <tr><td>https://api.dexko.co.kr/v2/public/orderbook</td><td>OrderBook</td></tr>
  <tr><td>https://api.dexko.co.kr/v2/public/transaction_history</td><td>Transaction History</td></tr>
  <tr><td>https://api.dexko.co.kr/v2/public/systemStatus</td><td>SystemStatus</td></tr>
  <tr><td>https://api.dexko.co.kr/v2/private/walletInfo</td><td>WalletAddress</td></tr>
  <tr><td>https://api.dexko.co.kr/v2/private/orderHis</td><td>OrderHis</td></tr>
  <tr><td>https://api.dexko.co.kr/v2/private/order</td><td>Order</td></tr>
  <tr><td>https://api.dexko.co.kr/v2/private/deleteOrder</td><td>Cancel</td></tr>
</table>


-------------
####  1. Market
  <p>Input Parameters: No</p>
  <p>Return Parameters</p>
  <table>
    <tr><th>Parameters</th><th>Date Type</th><th>Description</th></tr>
    <tr><td>market</td><td>String</td><td>Market Information</td></tr>
    <tr><td>korean_name</td><td>String</td><td>Cryptocurrency Korean</td></tr>
    <tr><td>english_name</td><td>String</td><td>Cryptocurrency English</td></tr>
    <tr><td>market_Id</td><td>String</td><td>Market ID</td></tr>
  </table>
  <pre>
  [
  {
    "MARKET":"BTC-ETH",
    "KOREAN_NAME":"이더리움",
    "ENGLISH_NAME":"ETH"
  },
  {
    "MARKET":"ETH-BTC",
    "KOREAN_NAME":"비트코인",
    "ENGLISH_NAME":"BTC"
  }
  ] 
  </pre>
  
  ####  2. Ticker
  <p>Input Parameters</p>
  <table>
    <tr><th>Parameters</th><th>Date Type</th><th>Description</th></tr>
    <tr><td>market</td><td>String</td><td>Market Group</td></tr>
  </table>
  <p>Return Parameters</p>
  <table>
    <tr><th>Parameters</th><th>Date Type</th><th>Description</th></tr>
    <tr><td>closing_price</td><td>Number(String)</td><td>Closing price 00:00 basis</td></tr>
    <tr><td>prev_closing_price</td><td>Number(String)</td><td>Previous day’s closing price</td></tr>
    <tr><td>date</td><td>String</td><td>Date time</td></tr>
    <tr><td>fluctuate_24h</td><td>Number(String)</td><td>The change in the last 24hours</td></tr>
    <tr><td>acc_trade_value</td><td>Number(String)</td><td>Volume 00:00 basis</td></tr>
    <tr><td>min_price</td><td>Number(String)</td><td>Low price 00:00 basis</td></tr>
    <tr><td>opening_price</td><td>Number(String)</td><td>Current Price 00:00 basis</td></tr>
    <tr><td>units_traded</td><td>Number(String)</td><td>Volume 00:00 basis</td></tr>
    <tr><td>units_traded_24h</td><td>Number(String)</td><td>Last 24hour volume</td></tr>
    <tr><td>fluctuate_rate_24h</td><td>Number(String)</td><td>Last 24hour volume change</td></tr>
    <tr><td>acc_trade_value_24h</td><td>Number(String)</td><td>Last 24hour trading amount</td></tr>
    <tr><td>max_price</td><td>Number(String)</td><td>High 00:00 basis</td></tr>
  </table>
  <pre>
  {
    "CLOSING_PRICE": 9735000,
    "PREV_CLOSING_PRICE": 9040000,
    "DATE": 1578448510137,
    "FLUCTATE_24H": 700000,
    "ACC_TRADE_VALUE": 37247083.5,
    "MIN_PRICE": 8885000,
    "OPENING_PRICE": 9735000,
    "UNITS_TRADED": 3.8261,
    "UNITS_TRADED_24H": 10.45288198,
    "FLUCTATE_RATE_24H": 0,
    "ACC_TRADE_VALUE_24H": 101654277.2555,
    "MAX_PRICE": 9735000
  }
  </pre>
  
  ####  3. OrderBook
  <p>Input Parameters</p>
  <table>
    <tr><th>Parameters</th><th>Date Type</th><th>Description</th></tr>
    <tr><td>market</td><td>String</td><td>Market Group</td></tr>
  </table>
  <p>Return Parameters</p>
  <table>
    <tr><th>Parameters</th><th>Date Type</th><th>Description</th></tr>
    <tr><td>bid</td><td>Array[Object]</td><td>Purchase request history</td></tr>
    <tr><td>quantity</td><td>Number(String)</td><td>Purchase Currency quantity</td></tr>
    <tr><td>price</td><td>Number(String)</td><td>Purchase Currency price</td></tr>
    <tr><td>ask</td><td>Array[Object]</td><td>Sell request history</td></tr>
    <tr><td>quantity</td><td>Number(String)</td><td>Sell Currency quantity</td></tr>
    <tr><td>price</td><td>Number(String)</td><td>Sell Currency price</td></tr>
  </table>
  <pre>
  {
    "result": {
        "ask": [
            {
                " PRICE": 9710000,
                " QUANTITY": 0.016
            },
            {
                " PRICE": 9700000,
                " QUANTITY ": 0.002
            },
            …….
        ],
        "bid": [
            {
                " PRICE": 4217000,
                " QUANTITY ": 2.186
            },
            {
                " PRICE": 4217000,
                " QUANTITY ": 1.96
            }
            ……..
        ]
    }
  }

  </pre>  
  
  ####  4. Transaction History
  <p>Input Parameters</p>
  <table>
    <tr><th>Parameters</th><th>Date Type</th><th>Description</th></tr>
    <tr><td>market</td><td>String</td><td>Market Group</td></tr>
  </table>
  <p>Return Parameters</p>
  <table>
    <tr><th>Parameters</th><th>Date Type</th><th>Description</th></tr>
    <tr><td>total</td><td>Number(String)</td><td>Total transaction amount</td></tr>
    <tr><td>transaction_date</td><td>String</td><td>Execution time</td></tr>
    <tr><td>price</td><td>Number(String)</td><td>Execution Price</td></tr>
    <tr><td>units_traded</td><td>Number(String)</td><td>Volume</td></tr>
    <tr><td>type</td><td>String</td><td>Transaction type(bid:purshase, ask:sell)</td></tr>
  </table>
  <pre>
  [
    {
        "TOTAL": 31878,
        "TRANSACTION_DATE": "2020-01-08 11:21:23",
        "PRICE": 9660000,
        "UNITS_TRADED": 0.0033,
        "TYPE": "BID"
    },
    {
        "TOTAL": 0.00001815,
        "TRANSACTION_DATE": "2020-01-08 11:21:23",
        "PRICE": 0.0033,
        "UNITS_TRADED": 0.0055,
        "TYPE": "ASK"
    },
    {
        "TOTAL": 11592,
        "TRANSACTION_DATE": "2020-01-08 11:21:15",
        "PRICE": 9660000,
        "UNITS_TRADED": 0.0012,
        "TYPE": "BID"
    },
    {
        "TOTAL": 0.0000066,
        "TRANSACTION_DATE": "2020-01-08 11:21:15",
        "PRICE": 0.0012,
        "UNITS_TRADED": 0.0055,
        "TYPE": "ASK"
    }
  ]

  </pre>  
  
  ####  5. SystemStatus
  <p>Input Parameters: No</p>
  <p>Return Parameters</p>
  <table>
    <tr><th>Parameters</th><th>Date Type</th><th>Description</th></tr>
    <tr><td>coin</td><td>String</td><td>Crytocurrency name</td></tr>
    <tr><td>assetType</td><td>String</td><td>Activation</td></tr>
    <tr><td>deposit</td><td>String</td><td>Market Status</td></tr>
    <tr><td>withdrawals</td><td>String</td><td>Withdrawals Status</td></tr>
    <tr><td>trading</td><td>String</td><td>Whether to trade</td></tr>
  <tr><td>url</td><td>String</td><td>Tracking address</td></tr>
  </table>
  <pre>
  [
    {
        "DEPOSITS": "Active",
        "ASSETTYPE": "Coin",
        "WITHDRAWALS": "Active",
        "TRADING": "Active",
        "COIN": "BTC",
        "URL": "https://btc.com/@transaction-id"
    },
    {
        "DEPOSITS": "Active",
        "ASSETTYPE": "Coin",
        "WITHDRAWALS": "Active",
        "TRADING": "Active",
        "COIN": "ETH",
        "URL": "https://etherscan.io/tx/@transaction-id"
    },
    {
        "DEPOSITS": "Active",
        "ASSETTYPE": "Coin",
        "WITHDRAWALS": "Active",
        "TRADING": "Active",
        "COIN": "BCH",
        "URL": "http://blockdozer.com/insight/tx/@transaction-id"
    }
  ]
  </pre>  
  
  
  ####  6. WalletAddress
  <p>Input Parameters</p>
  <table>
    <tr><th>Parameters</th><th>Date Type</th><th>Description</th></tr>
    <tr><td>authorization</td><td>String</td><td>Header(accessKey,nonce)</td></tr>
  </table>
  <p>Return Parameters</p>
  <table>
    <tr><th>Parameters</th><th>Date Type</th><th>Description</th></tr>
    <tr><td>Address</td><td>String</td><td>Wallet address</td></tr>
    <tr><td>Balance</td><td>String</td><td>Total amount</td></tr>
    <tr><td>Locked</td><td>String</td><td>The amount enclosed during the order</td></tr>
    <tr><td>Currency</td><td>String</td><td>an abbreviation for money on English</td></tr>
  </table>
  <pre>
  {
    "result": [
        {
            "CURRENCY": "KRW",
            "LOCKED": 51400,
            "ADDRESS": "35260101125712",
            "BALANCE": 229702.18600209
        },
        {
            "CURRENCY": "BTC",
            "LOCKED": 0,
            "ADDRESS": "3BHREtGG5z8sboFiQy3hvg8Lpmkwfo5omU",
            "BALANCE": 0.54346056
        },
        {
            "CURRENCY": "ETH",
            "LOCKED": 0,
            "ADDRESS": "0x3a388281ea636487b0fd86ea77b531132ee2bbec",
            "BALANCE": 10000941.43676287
        },
        {
            "CURRENCY": "HDAC",
            "LOCKED": 14,
            "ADDRESS": "4anHfn73MdqfomwLvsTfq5Ws7U5q4CS9Vs",
            "BALANCE": 100989.01
        }

    ]
  }

  </pre>

  ####  7. OrderHis
  <p>Input Parameters</p>
  <table>
    <tr><th>Parameters</th><th>Date Type</th><th>Description</th></tr>
    <tr><td>authorization</td><td>String</td><td>Header(accessKey,nonce)</td></tr>
    <tr><td>orderId</td><td>String</td><td>Order number(if none)</td></tr>
    <tr><td>market</td><td>String</td><td>unique key (KRW)</td></tr>
    <tr><td>currency</td><td>String</td><td>an abbreviation for money on English</td></tr>
    <tr><td>count</td><td>Number</td><td>Number of inquary (Default 100)</td></tr>
  </table>
  <p>Return Parameters</p>
  <table>
    <tr><th>Parameters</th><th>Date Type</th><th>Description</th></tr>
    <tr><td>ORDER_ID</td><td>String</td><td>Unique ID of the order</td></tr>
    <tr><td>SIDE</td><td>String</td><td>Order type ( B: Buy , S: Sell)</td></tr>
    <tr><td>ORD_TYPE</td><td>String</td><td>Order method (N:limits price)</td></tr>
    <tr><td>PRICE</td><td>String</td><td>The currency price at the time of order</td></tr>
    <tr><td>STATE</td><td>String</td><td>Order Status ( GO: Order , CC: Cancel, CM: Closed)</td></tr>
    <tr><td>MARKET</td><td>String</td><td>Market unique code</td></tr>
    <tr><td>CURRENCY</td><td>String</td><td>an abbreviation for money on English</td></tr>
    <tr><td>CREATED_AT</td><td>String</td><td>Order creation time</td></tr>
    <tr><td>VOLUME</td><td>String</td><td>Order quantity entered by the user</td></tr>
    <tr><td>REMAINING_VOLUME</td><td>String</td><td>Remaining order after order execution</td></tr>
    <tr><td>EXECUTED_VOLUME</td><td>String</td><td>Executed volume</td></tr>
  </table>
  <pre>
  {
    "result": [
        {
            "CURRENCY": "BTC",
            "SIDE": "B",
            "EXECUTED_VOLUME": 0,
            "MARKET": "KRW",
            "ORDER_ID": 40860911,
            "PRICE": 11210000,
            "CREATED_AT": "2019-07-31 09:33:36",
            "VOLUME": 0.0001,
            "STATE": "CC",
            "REMAINING_VOLUME": 0.0001,
            "ORD_TYPE": "N"
        },
        {
            "CURRENCY": "BTC",
            "SIDE": "B",
            "EXECUTED_VOLUME": 0.0001,
            "MARKET": "KRW",
            "ORDER_ID": 40860910,
            "PRICE": 12000000,
            "CREATED_AT": "2019-07-31 09:32:05",
            "VOLUME": 0.0001,
            "STATE": "CM",
            "REMAINING_VOLUME": 0,
            "ORD_TYPE": "N"
        },
        {
            "CURRENCY": "BTC",
            "SIDE": "B",
            "EXECUTED_VOLUME": 0.0001,
            "MARKET": "KRW",
            "ORDER_ID": 40858873,
            "PRICE": 22000000,
            "CREATED_AT": "2019-07-17 14:44:59",
            "VOLUME": 0.0001,
            "STATE": "CM",
            "REMAINING_VOLUME": 0,
            "ORD_TYPE": "N"
        }
    ]
  }
  </pre>
