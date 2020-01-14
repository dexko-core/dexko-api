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
  
  
  
  
  
  
  
  



<h3 id="server_url">Rest Api Url</h3>
S

<h3 id="contact_us">Contact Us</h3>
Message
