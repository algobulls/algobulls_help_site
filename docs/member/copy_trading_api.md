## AlgoBulls Copy Trading API Documentation

Version: 1.0, Revision 1.

<br>
----

### Order Placement API

Place main order of various types (regular, bracket, cover), various codes (intraday, delivery), across various segments (NSE, NFO, MCX, CDS) and across all supported Brokers on the AlgoBulls platform.

#### Curl Command:

```shell
# Sample Request
curl --location \
--request POST 'https://api.algobulls.com/v1/tr' \
--header 'Content-Type: application/json' \
--data-raw '{
    "key": "3ZPsvY18HyZbjCWdsyV5cl_OHNQ14Jc1BbAE7PJZSBKAR6MedAgJrkK9sLl3amDddRmqjw9Q2s25B2Vc2wd",
    "cmd": "ORDER_PLACEMENT",
    "instrument": {
        "segment": "NSE_FO",
        "exchangeToken": 3045
    },
    "quantity": 10,
    "position": "ENTRY",
    "orderTransactionType": "BUY",
    "orderVariety": "MARKET",
    "orderType": "REGULAR",
    "orderCode": "INTRADAY"
}'
```

```shell
# Sample response for success scenario
HTTP 200
{
    "message": "success",
    "orderId": "9a6e73ed8ac343be9e74bfc226ae1d21"
}
```

#### Description of parameters:

| Parameters    | Description           | Permissible Values  |
| ------------- |:-------------:| -----:|
| `key`      | Unique key provided by AlgoBulls. <br>This is linked to the strategy listed on the AlgoBulls marketplace | Should be a string |
| `cmd`      | Command for placing orders     | `"ORDER_PLACEMENT"`  |
| `instrument`:`segment`| Segment of the instrument      | Common names: `"NSE"`, `"NFO"`, `"NCD"`, `"MCX"`<br>Alternate names:`"NSE_EQ"`, `"NSE_FO"`, `"NSE_CD"`, `"MCX_FO"`|
| `instrument`:`exchangeToken` | A valid Exchange token of instrument | Should be a positive integer|
| `quantity` | Quantity of stock to be placed. <br><br>Depending on the mode set by client, either:<br> The exact quantity will be taken...<br> OR <br> A scaled up/down version of the quantity will be taken...<br> ...in the client's account | Should be a positive integer | 
| `position`| Expected position to be taken by this order. This can be either:<br>"ENTRY" when placing main orders<br>OR<br> "EXIT" when placing target/stoploss/exit orders   | `"ENTRY"`, `"EXIT"`|
| `orderTransactionType` | Order Transaction Type| `"BUY"`, `"SELL"`|
| `orderVariety` | Order Variety | Market: `"MARKET"` or `"M"`<br>Limit: `"LIMIT"` or `"L"`<br>Stoploss Limit: `"STOPLOSS"` or `"STOPLOSS_LIMIT"` or `"SL"`<br>Stoploss Market: `"STOPLOSS_MARKET"` or `"SLM"`|
| `orderType`| Order Type | `"REGULAR"`, `"BRACKET"`, `"COVER"`|
| `orderCode`| Order Code | `"INTRADAY"`, `"DELIVERY"`|
|`price`*| Limit Price | Should be a positive integer or float|
|`triggerPrice`* | Trigger Price | Should be a positive integer or float|
|`stoplossTrigger`*| Stoploss Trigger Price for Bracket Orders | Should be a positive integer or float|
|`targetTrigger`*| Target Trigger Price for Bracket Orders | Should be a positive integer or float|
|`trailingStoplossTrigger`*| Trailing Stoploss Trigger Price for Bracket Orders | Should be a positive integer or float|
|`relatedOrder`+| Order ID of a main order placed earlier for which this a corresponding exit order. | Should be a string |

*These parameters are only applicable for those order varieties and order codes where it makes sense. For those where it doesn't, you should skip these parameters.

+This is applicable only while placing orders with `"position"` as `"EXIT"`. This parameter should be skipped if not applicable 

----
<br>

### Order Cancellation API

Cancel any cancellable order placed using the AlgoBulls Order Placement API.

#### Curl Command:

```shell
# Sample Request
curl --location \
--request POST 'https://api.algobulls.com/v1/tr' \
--header 'Content-Type: application/json' \
--data-raw '{
    "key": "3ZPsvY18HyZbjCWdsyV5cl_OHNQ14Jc1BbAE7PJZSBKAR6MedAgJrkK9sLl3amDddRmqjw9Q2s25B2Vc2wd",
    "cmd": "ORDER_CANCELLATION",
    "orderId": "9a6e73ed8ac343be9e74bfc226ae1d21"
}'
```

```shell
# Sample response for success scenario
HTTP 200
{
    "message": "success",
}
```

#### Description of parameters:

| Parameters    | Description           | Permissible Values  |
| ------------- |:-------------:| -----:|
| `key`      | Unique key provided by AlgoBulls. <br>This is linked to the strategy listed on the AlgoBulls marketplace | Should be a string |
| `cmd`      | Command for cancelling orders     | `"ORDER_CANCELLATION"`  |
|`orderID`| Order ID of an order placed earlier using the AlgoBulls Order Placement API | Should be a string |

----
<br>

### Order Position Exit API

Exit position corresponding to an order placed using the AlgoBulls Order Placement API. This API ensures that position is smartly exited and no extra orders are placed to get a position exited in unexpected scenarios like order rejection, manual
exits, etc.

#### Curl Command:

```shell
# Sample Request
curl --location \
--request POST 'https://api.algobulls.com/v1/tr' \
--header 'Content-Type: application/json' \
--data-raw '{
    "key": "3ZPsvY18HyZbjCWdsyV5cl_OHNQ14Jc1BbAE7PJZSBKAR6MedAgJrkK9sLl3amDddRmqjw9Q2s25B2Vc2wd",
    "cmd": "ORDER_POSITION_EXIT",
    "orderId": "9a6e73ed8ac343be9e74bfc226ae1d21"
}'
```

```shell
# Sample response for success scenario
HTTP 200
{
    "message": "success",
}
```

#### Description of parameters:

| Parameters    | Description           | Permissible Values  |
| ------------- |:-------------:| -----:|
| `key`      | Unique key provided by AlgoBulls. <br>This is linked to the strategy listed on the AlgoBulls marketplace | Should be a string |
| `cmd`      | Command for exiting position corresponding to a main orders     | `"ORDER_POSITION_EXIT"`  |
|`orderID`| Order ID of an order placed earlier using the AlgoBulls Order Placement API | Should be a string |

----

```
Tip: To import any requests from this doc to your Postman app, you can do the following:
1. Copy the required cURL command from this doc.
2. Open POSTMAN
3. Click on "Import" button on the upper left side
4. Select the "Raw Text" option and paste your cURL command
5. Hit import
```

---