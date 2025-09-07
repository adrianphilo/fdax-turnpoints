#Columsn der Kennzahlenliste als Basis der Featureliste#

| Column | Description |
| ----- | ----- |
| **Block-Level Features** | \--- |
| `timeLastStr` | Timestamp of the last trade in the block (string format). |
| `timediff` | The time duration of the current block in seconds. |
| `timescore` | A score inversely proportional to the block's time duration (higher score for faster blocks). |
| `prcdiff` | Price change from the last price of the previous block to the last price of the current block. |
| `prcgrad` | The gradient (slope) of the price change over time within the block. |
| `volSum` | The total traded volume (sum of contracts) within the block. |
| `timeLast` | Timestamp of the last trade in the block (Unix milliseconds). |
| `priceLast` | The last traded price in the block. |
| `priceAvgXX` | A moving average price over a certain period (`XX` trades). |
| `priceMean` | The mean price of all trades within the current block. |
| `priceMin` | The minimum price recorded within the block. |
| `priceMax` | The maximum price recorded within the block. |
| `priceScore` | A score based on the price movement within the block. |
| **Future-Looking Features** | \--- |
| `timein50Str` | Timestamp in 50 trades from now (string format). |
| `timein50` | Timestamp in 50 trades from now (Unix milliseconds). |
| `pricein50` | The price in 50 trades from now. |
| `min50` | The minimum price over the next 50 trades. |
| `max50` | The maximum price over the next 50 trades. |
| `timein250Str` | Timestamp in 250 trades from now (string format). |
| `pricein250` | The price in 250 trades from now. |
| `min250` | The minimum price over the next 250 trades. |
| `max250` | The maximum price over the next 250 trades. |
| `timein500Str` | Timestamp in 500 trades from now (string format). |
| `pricein500` | The price in 500 trades from now. |
| `min500` | The minimum price over the next 500 trades. |
| `max500` | The maximum price over the next 500 trades. |
| `timein1000Str` | Timestamp in 1000 trades from now (string format). |
| `pricein1000` | The price in 1000 trades from now. |
| `min1000` | The minimum price over the next 1000 trades. |
| `max1000` | The maximum price over the next 1000 trades. |
| **Past-Looking Features (250 Trades Ago)** | \--- |
| `ago250timeStr` | Timestamp 250 trades ago (string format). |
| `ago250price` | The price 250 trades ago. |
| `ago250diff` | The price change in the block that occurred 250 trades ago. |
| `ago250grad` | The price gradient in the block that occurred 250 trades ago. |
| `ago250diffAct` | The difference between the current price and the price 250 trades ago. |
| **Moving Average Features (250 Trades)** | \--- |
| `avg250min` | Minimum value of the 250-trade moving average. |
| `avg250max` | Maximum value of the 250-trade moving average. |
| `avg250siz` | Total volume over the last 250 trades. |
| `avg250wavg` | The volume-weighted average price over the last 250 trades. |
| `avg250diff` | The change in the 250-trade moving average from the previous block. |
| `avg250grad` | The gradient (slope) of the 250-trade moving average. |
| `avg250diffAct` | The difference between the current price and the 250-trade moving average. |
| `avg250crossAct` | An event flag for the current price crossing the 250-trade moving average. |
| **Past-Looking & Moving Average Features (1000 Trades)** | \--- |
| `ago1000timeStr` | Timestamp 1000 trades ago (string format). |
| `ago1000price` | The price 1000 trades ago. |
| `ago1000diff` | The price change in the block that occurred 1000 trades ago. |
| `ago1000grad` | The price gradient in the block that occurred 1000 trades ago. |
| `ago1000diffAct` | The difference between the current price and the price 1000 trades ago. |
| `avg1000wavg` | The volume-weighted average price over the last 1000 trades. |
| `avg1000diff` | The change in the 1000-trade moving average from the previous block. |
| `avg1000grad` | The gradient (slope) of the 1000-trade moving average. |
| `avg1000diffAct` | The difference between the current price and the 1000-trade moving average. |
| `avg1000crossAct` | An event flag for the current price crossing the 1000-trade moving average. |
| **Trigger & Normalized Features** | \--- |
| `trigger250` | A binary flag indicating a potential turning point within the next 250 trades. |
| `trigger500` | A binary flag indicating a potential turning point within the next 500 trades. |
| `trigger1000` | A binary flag indicating a potential turning point within the next 1000 trades. |
| `priceMin0` | The minimum price of the block, relative to its first trade. |
| `priceMax0` | The maximum price of the block, relative to its first trade. |
| `priceMean0` | The mean price of the block, relative to its first trade. |
| `avg250wavg0` | The 250-trade weighted average, relative to the block's first trade. |
| `avg1000wavg0` | The 1000-trade weighted average, relative to the block's first trade. |
| `pricein250n` | The price in 250 trades, normalized. |
| `pricein1000n` | The price in 1000 trades, normalized. |
| `avg250wavgDif` | The difference between the current price and the 250-trade weighted average. |
| `avg1000wavgDif` | The difference between the current price and the 1000-trade weighted average. |
| `pricein250dif` | The difference between the current price and the price in 250 trades. |
| `min250_` | The minimum price over the next 250 trades, normalized. |
| `max250_` | The maximum price over the next 250 trades, normalized. |
| `min500_` | The minimum price over the next 500 trades, normalized. |
| `max500_` | The maximum price over the next 500 trades, normalized. |
| `min1000_` | The minimum price over the next 1000 trades, normalized. |
| `max1000_` | The maximum price over the next 1000 trades, normalized. |
