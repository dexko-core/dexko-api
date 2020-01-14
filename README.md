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
#### Market
  <p>Input Parameters: No</p>
  <p>Return Parameters</p>
  <table>
    <tr><th>Parameters</th><th>Date Type</th><th>Description</th></tr>
    <tr><td>market</td><td>String</td><td>Market Information</td></tr>
    <tr><td>korean_name</td><td>String</td><td></td></tr>
    <tr><td>english_name</td><td>String</td><td></td></tr>
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
  
  
  
  
  
  
  
  
  
  



<h3 id="server_url">Rest Api Url</h3>
S

<h3 id="contact_us">Contact Us</h3>
Message
