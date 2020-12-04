---
description: ARS configurable variables
---

# ARS Variables

## Bot Parameters

### BIN\_NAME

{% tabs %}
{% tab title="Description" %}
Should be changed for non BTC pairs
{% endtab %}

{% tab title="Values" %}
Default Value: "USDT-BTC"
{% endtab %}
{% endtabs %}

### BINANCE

{% tabs %}
{% tab title="Description" %}
Use Binance to calculate PPP Index on 1 hour time frame. If disabled - using 1 mknute time frame.
{% endtab %}

{% tab title="Values" %}
Default Value: True
{% endtab %}
{% endtabs %}

## Pair Parameters

{% hint style="info" %}
These settings should be prefaced with \[pair\].settings.\[variable\]

For example: USDTBTC.settings.MAX\_BUY
{% endhint %}

### MAX\_BUY

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Default GB value
{% endtab %}

{% tab title="Values" %}
Default Value: 0
{% endtab %}
{% endtabs %}

### MAX\_SELL

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Default GB value
{% endtab %}

{% tab title="Values" %}
Default Value: 0
{% endtab %}
{% endtabs %}

### TRADING\_LIMIT

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Calculated automatically in ARS, however if TL\_AT set to False - this will be respected
{% endtab %}

{% tab title="Values" %}
Default Value: 15
{% endtab %}
{% endtabs %}

### UTA\_PERIOD

{% tabs %}
{% tab title="Description" %}
Default UTA period ARS start with when no position opened
{% endtab %}

{% tab title="Values" %}
Default Value: 1
{% endtab %}
{% endtabs %}

### MAX\_OPEN\_CONTRACTS

{% tabs %}
{% tab title="Description" %}
MOC for GB. High value used to never be triggered as ARS use own protection. Could be changed to user defined value.
{% endtab %}

{% tab title="Values" %}
Default Value: 10000000
{% endtab %}
{% endtabs %}

### REDUCING\_RATIO

{% tabs %}
{% tab title="Description" %}
RR for HR, Using 1 to close entire position if ARS protection triggered
{% endtab %}

{% tab title="Values" %}
Default Value: 1
{% endtab %}
{% endtabs %}

### UNLIMITED\_POSITION\_SIZE

{% tabs %}
{% tab title="Description" %}
Safe position size when ARS ignores the protection. It recalcuates inside ARS, but will respect user defined value if you set it.
{% endtab %}

{% tab title="Values" %}
Default Value: 0.0001
{% endtab %}
{% endtabs %}

### LIQUIDATION\_STOP

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Liq Limit value where DCA\_EMA changes EMA spread
{% endtab %}

{% tab title="Values" %}
Default Value: 80
{% endtab %}
{% endtabs %}

### LIQUIDATION\_LIMIT

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Default Liquidation Limit. When reached - position freeze
{% endtab %}

{% tab title="Values" %}
Default Value: 80
{% endtab %}
{% endtabs %}

### LIQUIDATION\_WAIT

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Wait time between Slice of Limit
{% endtab %}

{% tab title="Values" %}
Default Value: 15
{% endtab %}
{% endtabs %}

### LIQUIDATION\_SLICE

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Limit Slice size
{% endtab %}

{% tab title="Values" %}
Default Value: 2
{% endtab %}
{% endtabs %}

### PRICE\_DELTA\_LIMIT

{% tabs %}
{% tab title="Description" %}
Delta between last candle close and current ASK in 1 min frame. Used as one of PDP triggers.
{% endtab %}

{% tab title="Values" %}
Default Value: 0.4
{% endtab %}
{% endtabs %}

### PDP\_UPNL\_LIMIT

{% tabs %}
{% tab title="Description:" %}
Allowed % loss of your wallet when PDP trying to close position against market move. If loss will be higher then this value - ARS will not close position
{% endtab %}

{% tab title="Values" %}
Default Value: -1
{% endtab %}
{% endtabs %}

### PDP\_SLOW\_LIMIT

{% tabs %}
{% tab title="Description" %}
Allowed % loss of your wallet when PDP trying to close position against SLOW \(predictive\) market move
{% endtab %}

{% tab title="Values" %}
Default Value: -0.1
{% endtab %}
{% endtabs %}

### PDP\_VOL\_FAST

{% tabs %}
{% tab title="Description" %}
Pair volume - one of additional confirming PDP Indicators
{% endtab %}

{% tab title="Values" %}
Default Value: 10000000
{% endtab %}
{% endtabs %}

### PDP\_VOL\_SLOW

{% tabs %}
{% tab title="Description" %}
Pair volume - one of additional confirming PDP Indicators for SLOW move
{% endtab %}

{% tab title="Values" %}
Default Value: 10000000
{% endtab %}
{% endtabs %}

### PDP\_TL\_FACTOR

{% tabs %}
{% tab title="Description" %}
TL Factor use when position follow the Pump/Dump
{% endtab %}

{% tab title="Values" %}
Default Value: 4
{% endtab %}
{% endtabs %}

### PPP\_SIDE\_UPNL\_LIMIT

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Allowed % loss of your wallet when PPP closes position at loss in case of market exit from Side and position againts PPP Index
{% endtab %}

{% tab title="Values" %}
Default Value: -0.5
{% endtab %}
{% endtabs %}

### PPP\_UPNL\_LIMIT

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Allowed % loss of your wallet when PPP closes position at loss because PPP Index changes
{% endtab %}

{% tab title="Values" %}
Default Value: -1
{% endtab %}
{% endtabs %}

### DELAY\_HIGH

{% tabs %}
{% tab title="Description" %}
Default GB delay
{% endtab %}

{% tab title="Values" %}
Default Value: 12
{% endtab %}
{% endtabs %}

### DELAY\_LOW

{% tabs %}
{% tab title="Description" %}
Delay use to trail position - when MAX BS disabled and extremely low Delay used to catch the spikes and close position with best ROE
{% endtab %}

{% tab title="Values" %}
Default Value: 8
{% endtab %}
{% endtabs %}

### TLX

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Auto TL factor. Used with Mode 2 to increase Auto TL x times
{% endtab %}

{% tab title="Values" %}
Default Value: 1
{% endtab %}
{% endtabs %}

### SPK\_KILL

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Small Position Killer ROE value - if below this ROE for Time below - closing at loss
{% endtab %}

{% tab title="Values" %}
Default Value: -100
{% endtab %}
{% endtabs %}

### SPK\_TIME

{% tabs %}
{% tab title="First Tab" %}
Time trigger for SPK function above
{% endtab %}

{% tab title="Second Tab" %}
Default Value: 15
{% endtab %}
{% endtabs %}

### ROE

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Default ROE value
{% endtab %}

{% tab title="Values" %}
Default Value: 8
{% endtab %}
{% endtabs %}

### ROE\_LIMIT

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Default Limit value
{% endtab %}

{% tab title="Values" %}
Default Value: 2
{% endtab %}
{% endtabs %}

### PDP\_ROE

{% tabs %}
{% tab title="Description" %}
Increased ROE when we are inside Pump/Dump
{% endtab %}

{% tab title="Values" %}
Default Value: 20
{% endtab %}
{% endtabs %}

### PDP\_ROE\_LIMIT

{% tabs %}
{% tab title="Description" %}
Increased ROE Limit when we are inside Pump/Dump
{% endtab %}

{% tab title="Values" %}
Default Value: 5
{% endtab %}
{% endtabs %}

### UNLIM\_ROE\_LOW

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
ROE period where we don’t allow to DCA \(because no reason while price is close to 0\)
{% endtab %}

{% tab title="Values" %}
Default Value: -20
{% endtab %}
{% endtabs %}

### UNLIM\_ROE\_HIGH

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
ROE period where we don’t allow to DCA \(because no reason while price is close to 0\)
{% endtab %}

{% tab title="Values" %}
Default Value: -2
{% endtab %}
{% endtabs %}

### DCA\_EMA

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
DCA by EMA blocker
{% endtab %}

{% tab title="Values" %}
Default Value: True
{% endtab %}
{% endtabs %}

### SPK

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Small Position Killer ROE value - if below this ROE for Time below - closing at loss
{% endtab %}

{% tab title="Values" %}
Default Value: True
{% endtab %}
{% endtabs %}

### PDP

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Pump / Dump Protection
{% endtab %}

{% tab title="Values" %}
Default Value: True
{% endtab %}
{% endtabs %}

### PPP

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Passive Position Protection
{% endtab %}

{% tab title="Values" %}
Default Value: True
{% endtab %}
{% endtabs %}

### pSar

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
PPP Index calculation
{% endtab %}

{% tab title="Values" %}
Default Value: True
{% endtab %}
{% endtabs %}

### TL\_AC

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Auto TL
{% endtab %}

{% tab title="Values" %}
Default Value: True
{% endtab %}
{% endtabs %}

### AT\_DL

{% tabs %}
{% tab title="Description" %}
ARS Trailing function
{% endtab %}

{% tab title="Values" %}
Default Value: True
{% endtab %}
{% endtabs %}

### AUTO\_DISABLE

{% tabs %}
{% tab title="Description" %}
Auto Disable pair when position closes
{% endtab %}

{% tab title="Values" %}
Default Value: False
{% endtab %}
{% endtabs %}

### DCA\_FORCE

{% tabs %}
{% tab title="Description" %}
Force DCA ignoring everything but LIQUIDATION LIMIT
{% endtab %}

{% tab title="Values" %}
Default Value: False
{% endtab %}
{% endtabs %}

### PRE\_ORDER

{% tabs %}
{% tab title="Description" %}
Use Pre Order Gap
{% endtab %}

{% tab title="Values" %}
Default Value: False
{% endtab %}
{% endtabs %}

### PRE\_ORDER\_SR

{% tabs %}
{% tab title="Description" %}
Use Pre Order Gap to ask like SR \(not replacing ROE close\)
{% endtab %}

{% tab title="Values" %}
Default Value: False
{% endtab %}
{% endtabs %}

### ROE\_PRE\_ORDER\_SR

{% tabs %}
{% tab title="Description" %}
ROE below which we allow Pre Order to close positions
{% endtab %}

{% tab title="Values" %}
Default Value: 0.5
{% endtab %}
{% endtabs %}

### SR\_TRAIL

{% tabs %}
{% tab title="Description" %}
Use SR to trail position \(ROE close will not be used\)
{% endtab %}

{% tab title="Values" %}
Default Value: False
{% endtab %}
{% endtabs %}

### SR\_SWITCH

{% tabs %}
{% tab title="Description" %}
Enable and Disable SR
{% endtab %}

{% tab title="Values" %}
Default Value: True
{% endtab %}
{% endtabs %}

### SR\_RATE\_CHANGE

{% tabs %}
{% tab title="Description" %}
Sr rate changing to value below on side market and back to 1 if not side. Useful for KF
{% endtab %}

{% tab title="Values" %}
Default Value: False
{% endtab %}
{% endtabs %}

### SR\_RATIO\_TRAIL

{% tabs %}
{% tab title="Description" %}
SR\_RATE on Side if enabled above
{% endtab %}

{% tab title="Values" %}
Default Value: 1.40
{% endtab %}
{% endtabs %}

### SR\_RATIO\_COMMON

{% tabs %}
{% tab title="Description" %}
SR\_RATE if enabled above
{% endtab %}

{% tab title="Values" %}
Default Value: 1
{% endtab %}
{% endtabs %}

### UTA\_SKIP

{% tabs %}
{% tab title="Description" %}
ignore UTA
{% endtab %}

{% tab title="Values" %}
Default Value: False
{% endtab %}
{% endtabs %}

### TL\_AC\_PRICE

{% tabs %}
{% tab title="Description" %}
Use improved Auto TL formula which take BTC price into consideration
{% endtab %}

{% tab title="Values" %}
Default Value: False
{% endtab %}
{% endtabs %}

### PDP\_NO\_ROE\_CLOSE

{% tabs %}
{% tab title="Description" %}
Increases the ROE and Trailing to the values below to not to close the Position fast when we riding pump/dump
{% endtab %}

{% tab title="Values" %}
Default Value: False
{% endtab %}
{% endtabs %}

### PDP\_ROE\_NRC

{% tabs %}
{% tab title="Description" %}
Increased values for function above
{% endtab %}

{% tab title="Values" %}
Default Value: 200
{% endtab %}
{% endtabs %}

### PDP\_ROE\_LIMIT\_NRC

{% tabs %}
{% tab title="Description" %}
Increased values for function above
{% endtab %}

{% tab title="Values" %}
Default Value: 50
{% endtab %}
{% endtabs %}

### NO\_MARKET\_ORDERS

{% tabs %}
{% tab title="Description" %}
Don’t close at market when we trail position
{% endtab %}

{% tab title="Values" %}
Default Value: False
{% endtab %}
{% endtabs %}

### RB\_FORCE\_CLOSE

{% tabs %}
{% tab title="Description" %}
One time function to close position at loss using RebatesBuster
{% endtab %}

{% tab title="Values" %}
Default Value: False
{% endtab %}
{% endtabs %}

### NO\_STUCK

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Ignored next values if enabled and just closed at any loss when triggered: PDP\_UPNL\_LIMIT PDP\_SLOW\_LIMIT PPP\_SIDE\_UPNL\_LIMIT PPP\_UPNL\_LIMIT
{% endtab %}

{% tab title="Values" %}
Default Value: False
{% endtab %}
{% endtabs %}

### TT\_LOCK

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Effective only on BinanceFutures - Don’t allow to post LONG orders when position is SHORT and vice versa if ROE between 0 and this TT\_LOCK
{% endtab %}

{% tab title="Values" %}
Default Value: 0.5
{% endtab %}
{% endtabs %}

### ISL\_LIQ\_IGNORE

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Ignore the Liquidation Spread untill this wallet allocation % reached. Effective on KrakenFutured, never use it on bitmex and only with low leverage on binance Futures. To disable set 0
{% endtab %}

{% tab title="Values" %}
Default Value: 5
{% endtab %}
{% endtabs %}

### GRID

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
If enabled Only GRID - used mixed MM+GRID mode called "MODE 2", if Disabled - ARS uses old good MM only mode called "MODE 1\)
{% endtab %}

{% tab title="Values" %}
Default Value: False
{% endtab %}
{% endtabs %}

### x125

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Not effective alone. If set with GRID will enabled Gunthars Beast mode \(using MM and GRID same time with leverage 125\),called "MODE 3"
{% endtab %}

{% tab title="Values" %}
Default Value: False
{% endtab %}
{% endtabs %}

### NO\_SIDE\_LOCK

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
Don’t block position on side market when Unrealised PNL is 0.5% \(by default it does to be able to close with small loss if we exit side market against PPP index\)
{% endtab %}

{% tab title="Values" %}
Default Value: False
{% endtab %}
{% endtabs %}

### TRADE\_SIDE\_LOCK

{% hint style="info" %}

{% endhint %}

{% tabs %}
{% tab title="Description" %}
You could force lock ARS to only once side trading forever \(always LONG or always SHORT\)
{% endtab %}

{% tab title="Values" %}
Default Value: "None"
{% endtab %}
{% endtabs %}

