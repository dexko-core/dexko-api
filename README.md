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
    <tr><td></td><td></td><td></td></tr>
  </table>
  
  <table class=MsoTableGrid border=1 cellspacing=0 cellpadding=0
 style='border-collapse:collapse;border:none;mso-border-alt:solid windowtext .5pt;
 mso-yfti-tbllook:1184;mso-padding-alt:0cm 5.4pt 0cm 5.4pt'>
 <tr style='mso-yfti-irow:0;mso-yfti-firstrow:yes;mso-yfti-lastrow:yes'>
  <td width=1008 valign=top style='width:756.3pt;border:solid windowtext 1.0pt;
  mso-border-alt:solid windowtext .5pt;padding:0cm 5.4pt 0cm 5.4pt'><pre
  style='vertical-align:baseline'><span class=bggray><span lang=EN-US
  style='font-size:9.0pt;color:#777777'>[<o:p></o:p></span></span></pre><pre
  style='vertical-align:baseline'><span class=bggray><span lang=EN-US
  style='font-size:9.0pt;color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp; </span>{<o:p></o:p></span></span></pre><pre
  style='vertical-align:baseline'><span class=bggray><span lang=EN-US
  style='font-size:9.0pt;color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>&quot;MARKET&quot;: &quot;KRW-ETH&quot;,<o:p></o:p></span></span></pre><pre
  style='vertical-align:baseline'><span class=bggray><span lang=EN-US
  style='font-size:9.0pt;color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>&quot;KOREAN_NAME&quot;: &quot;</span></span><span
  class=bggray><span style='font-size:9.0pt;'>이더리움</span></span><span
  class=bggray><span lang=EN-US style='font-size:9.0pt;
  color:#777777'>&quot;,<o:p></o:p></span></span></pre><pre style='vertical-align:
  baseline'><span class=bggray><span lang=EN-US style='font-size:9.0pt;
  color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>&quot;ENGLISH_NAME&quot;: &quot;ETH&quot;,<o:p></o:p></span></span></pre><pre
  style='text-indent:36.0pt;mso-char-indent-count:4.0;vertical-align:baseline'><span
  class=bggray><span lang=EN-US style='font-size:9.0pt;
  color:#777777'>&quot;MARKET_ID&quot;: &quot;2&quot;<o:p></o:p></span></span></pre><pre
  style='vertical-align:baseline'><span class=bggray><span lang=EN-US
  style='font-size:9.0pt;color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp; </span>},<o:p></o:p></span></span></pre><pre
  style='vertical-align:baseline'><span class=bggray><span lang=EN-US
  style='font-size:9.0pt;color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp; </span>{<o:p></o:p></span></span></pre><pre
  style='vertical-align:baseline'><span class=bggray><span lang=EN-US
  style='font-size:9.0pt;color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>&quot;MARKET&quot;: &quot;KRW-HDAC&quot;,<o:p></o:p></span></span></pre><pre
  style='vertical-align:baseline'><span class=bggray><span lang=EN-US
  style='font-size:9.0pt;color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>&quot;KOREAN_NAME&quot;: &quot;</span></span><span
  class=bggray><span style='font-size:9.0pt;'>에이치닥</span></span><span
  class=bggray><span lang=EN-US style='font-size:9.0pt;'>&quot;,<o:p></o:p></span></span></pre><pre style='vertical-align:
  baseline'><span class=bggray><span lang=EN-US style='font-size:9.0pt;
 color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>&quot;ENGLISH_NAME&quot;: &quot;HDAC&quot;,<o:p></o:p></span></span></pre><pre
  style='text-indent:36.0pt;mso-char-indent-count:4.0;vertical-align:baseline'><span
  class=bggray><span lang=EN-US style='font-size:9.0pt;color:#777777'>&quot;MARKET_ID&quot;: &quot;3&quot;<o:p></o:p></span></span></pre><pre
  style='vertical-align:baseline'><span class=bggray><span lang=EN-US
  style='font-size:9.0pt;color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp; </span>},<o:p></o:p></span></span></pre><pre
  style='vertical-align:baseline'><span class=bggray><span lang=EN-US
  style='font-size:9.0pt;color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp; </span>{<o:p></o:p></span></span></pre><pre
  style='vertical-align:baseline'><span class=bggray><span lang=EN-US
  style='font-size:9.0pt;color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>&quot;MARKET&quot;: &quot;KRW-QTUM&quot;,<o:p></o:p></span></span></pre><pre
  style='vertical-align:baseline'><span class=bggray><span lang=EN-US
  style='font-size:9.0pt;color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>&quot;KOREAN_NAME&quot;: &quot;</span></span><span
  class=bggray><span style='font-size:9.0pt;color:#777777'>퀀텀</span></span><span
  class=bggray><span lang=EN-US style='font-size:9.0pt;color:#777777'>&quot;,<o:p></o:p></span></span></pre><pre style='vertical-align:
  baseline'><span class=bggray><span lang=EN-US style='font-size:9.0pt; color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>&quot;ENGLISH_NAME&quot;: &quot;QTUM&quot;,<o:p></o:p></span></span></pre><pre
  style='text-indent:36.0pt;mso-char-indent-count:4.0;vertical-align:baseline'><span
  class=bggray><span lang=EN-US style='font-size:9.0pt; color:#777777'>&quot;MARKET_ID&quot;: &quot;4&quot;<o:p></o:p></span></span></pre><pre
  style='vertical-align:baseline'><span class=bggray><span lang=EN-US
  style='font-size:9.0pt;color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp; </span>},<o:p></o:p></span></span></pre><pre
  style='vertical-align:baseline'><span class=bggray><span lang=EN-US
  style='font-size:9.0pt;color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp; </span>{<o:p></o:p></span></span></pre><pre
  style='vertical-align:baseline'><span class=bggray><span lang=EN-US
  style='font-size:9.0pt;color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>&quot;MARKET&quot;: &quot;KRW-BTC&quot;,<o:p></o:p></span></span></pre><pre
  style='vertical-align:baseline'><span class=bggray><span lang=EN-US
  style='font-size:9.0pt;color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>&quot;KOREAN_NAME&quot;: &quot;</span></span><span
  class=bggray><span style='font-size:9.0pt;color:#777777'>비트코인</span></span><span
  class=bggray><span lang=EN-US style='font-size:9.0pt; color:#777777'>&quot;,<o:p></o:p></span></span></pre><pre style='vertical-align:
  baseline'><span class=bggray><span lang=EN-US style='font-size:9.0pt;color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; </span>&quot;ENGLISH_NAME&quot;: &quot;BTC&quot;,<o:p></o:p></span></span></pre><pre
  style='text-indent:36.0pt;mso-char-indent-count:4.0;vertical-align:baseline'><span
  class=bggray><span lang=EN-US style='font-size:9.0pt;color:#777777'>&quot;MARKET_ID&quot;: &quot;1&quot;<o:p></o:p></span></span></pre><pre
  style='vertical-align:baseline'><span class=bggray><span lang=EN-US
  style='font-size:9.0pt;color:#777777'><span style='mso-spacerun:yes'>&nbsp;&nbsp;&nbsp; </span>}<o:p></o:p></span></span></pre><pre
  style='vertical-align:baseline;word-break:break-hangul'><span class=bggray><span
  lang=EN-US style='font-size:9.0pt;color:#777777'>]<o:p></o:p></span></span></pre></td>
 </tr>
</table>
  
  
  
  
  
  
  
  
  
  
  



<h3 id="server_url">Rest Api Url</h3>
S

<h3 id="contact_us">Contact Us</h3>
Message
