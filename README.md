# DEXKO API 

<p>Getting Started Guide</p>
<ul>
<li><a href="#create_key">Create API Key</a></li>
<li><a href="#server_url">REST API URL</a></li>
<li><a href="#contact_us">Contact Us</a></li>
</ul>
<h3 id="create_key">Create API Key</h3>
Create API

<h3>API List</h3>
<table>
  <tr><th>URL</th><th>Description</th></tr>
  <tr><td>https://api.dexko.co.kr/v2/public/market/all</td><td>Get market information</td></tr>
  <tr><td>https://api.dexko.co.kr/v2/public/ticker</td><td>Current a tick</td></tr>
  <tr><td>https://api.dexko.co.kr/v2/public/orderbook</td><td>Get Orderbook</td></tr>
  <tr><td>https://api.dexko.co.kr/v2/public/transaction_history</td><td>Get history of transactions</td></tr>
  <tr><td>https://api.dexko.co.kr/v2/public/systemStatus</td><td>Get the current status of system</td></tr>
  
  
  <tr><td>https://api.dexko.co.kr/v2/private/walletInfo</td><td>Get the information of person's wallet</td></tr>
  <tr><td>https://api.dexko.co.kr/v2/public/market/all</td><td>Get market information</td></tr>
</table>

<h3>Get Market List<h3>
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
