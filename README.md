# Arbidex-show-more-info
Bookmarlet to show/hide totals and percentages for each week for the arbitrage, in arbidex account balances section.

## What it does
Basicaly this adds a extra column in the `Arbitrage History table`, showing the totals of each week, and the % of increment.
When executed again, it should delete all added information, and go back to normal state.

![New column after running script](https://tomyo.github.io/arbidex-show-more-info/ABX_arbitrage_extra_column.png)

## How it's done
This is done backtracking from the current balance, substracting the profits each week, calculating each previous total and percentage.

## Why?
* I wanted to see for my self the profits percentage each week, and didn't wanted to do it manualy in a sheet.
* I wanted this information to be part of the UI of Arbidex.
* I wanted to know if the global profits reported by Arbidex [here](https://kb.arbidex.uk.com/knowledge-base/arbitrage-percentage-historical-data) were accurate. Not very much for me, what about you?

## How to use
There are three ways to use this:

1. Go [here](https://tomyo.github.io/arbidex-show-more-info/) and bookmark the link. or, 
2. Create a bookmark, pasting the link content in the `location` field:
```js
javascript:(function(){let newScript = document.createElement('script');newScript.src = 'https://tomyo.github.io/arbidex-show-more-info/arbidex-more-info.js';document.body.appendChild(newScript);})();)
```
3. Simply copy the code from https://github.com/tomyo/arbidex-show-more-info/blob/master/arbidex-more-info.js and paste it in the console.

* In every case, run the code/bookmarklet in the tab you have Arbidex open, in the account tab.

## Disclaimer
Use at your own risk, please read the code before executing it in your browser, as you should always do.

## Bugs?
I tested this in my account, only using ETH, it's probable that this will be buggy when using EHT abd BTC together.
Please feel free to report bugs, improvements, push requests, etc.

