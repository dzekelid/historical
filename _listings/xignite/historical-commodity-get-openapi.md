---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Futures Get Historical Commodity Chart
  description: Get a historical chart for a commodity.
  version: 1.0.0
host: www.xignite.com
basePath: xFutures.json/XigniteFutures
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ConvertHistoricalValue:
    get:
      summary: Convert Historical Value
      description: Convert value from one currency to another as of a historical date.
      operationId: postConverthistoricalvalue
      x-api-path-slug: converthistoricalvalue-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Convert
      - Historical
      - Value
  /GetHistoricalCrossRateTables:
    get:
      summary: Get Historical Cross Rate Tables
      description: Returns historical currency cross-rate tables for a range of dates.
      operationId: postGethistoricalcrossratetables
      x-api-path-slug: gethistoricalcrossratetables-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rate
      - Tables
  /GetHistoricalCrossRateTablesBidAsk:
    get:
      summary: Get Historical Cross Rate Tables Bid Ask
      description: Returns historical currency cross-rate tables for a range of dates.
      operationId: postGethistoricalcrossratetablesbask
      x-api-path-slug: gethistoricalcrossratetablesbidask-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rate
      - Tables
      - Bid
      - Ask
  /GetHistoricalCrossRateTable:
    get:
      summary: Get Historical Cross Rate Table
      description: Returns a historical currency cross-rate table.
      operationId: postGethistoricalcrossratetable
      x-api-path-slug: gethistoricalcrossratetable-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rate
      - Table
  /GetHistoricalCrossRateTableBidAsk:
    get:
      summary: Get Historical Cross Rate Table Bid Ask
      description: Returns a historical currency cross-rate table.
      operationId: postGethistoricalcrossratetablebask
      x-api-path-slug: gethistoricalcrossratetablebidask-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rate
      - Table
      - Bid
      - Ask
  /GetHistoricalCrossRateTableAsHTML:
    get:
      summary: Get Historical Cross Rate Table As H T M L
      description: Returns a historical currency cross-rate table as an HTML Output.
      operationId: postGethistoricalcrossratetableashtml
      x-api-path-slug: gethistoricalcrossratetableashtml-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rate
      - Table
      - As
      - H
      - T
      - M
      - L
  /GetHistoricalCrossRate:
    get:
      summary: Get Historical Cross Rate
      description: Returns a cross-rate as of a historical date.
      operationId: postGethistoricalcrossrate
      x-api-path-slug: gethistoricalcrossrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rate
  /GetHistoricalCrossRates:
    get:
      summary: Get Historical Cross Rates
      description: Returns multiple cross-rates as of a historical date.
      operationId: postGethistoricalcrossrates
      x-api-path-slug: gethistoricalcrossrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rates
  /GetHistoricalCrossRateBidAsk:
    get:
      summary: Get Historical Cross Rate Bid Ask
      description: Returns a cross-rate with bid/ask as of a historical date.
      operationId: postGethistoricalcrossratebask
      x-api-path-slug: gethistoricalcrossratebidask-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rate
      - Bid
      - Ask
  /GetHistoricalCrossRatesBidAsk:
    get:
      summary: Get Historical Cross Rates Bid Ask
      description: Returns multiple cross-rates with bid/ask as of a historical date.
      operationId: postGethistoricalcrossratesbask
      x-api-path-slug: gethistoricalcrossratesbidask-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rates
      - Bid
      - Ask
  /GetHistoricalCrossRatesRange:
    get:
      summary: Get Historical Cross Rates Range
      description: This operation returns a range of cross-rates for a currency pair.
      operationId: postGethistoricalcrossratesrange
      x-api-path-slug: gethistoricalcrossratesrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rates
      - Range
  /GetHistoricalCrossRatesBidAskRange:
    get:
      summary: Get Historical Cross Rates Bid Ask Range
      description: This operation returns a range of cross-rates for a currency pair.
      operationId: postGethistoricalcrossratesbaskrange
      x-api-path-slug: gethistoricalcrossratesbidaskrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rates
      - Bid
      - Ask
      - Range
  /GetHistoricalCrossRatesAsOf:
    get:
      summary: Get Historical Cross Rates As Of
      description: This operation returns a range of cross-rates for a currency pair.
      operationId: postGethistoricalcrossratesasof
      x-api-path-slug: gethistoricalcrossratesasof-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rates
      - As
      - Of
  /GetHistoricalCrossRatesBidAskAsOf:
    get:
      summary: Get Historical Cross Rates Bid Ask As Of
      description: This operation returns a range of cross-rates for a currency pair.
      operationId: postGethistoricalcrossratesbaskasof
      x-api-path-slug: gethistoricalcrossratesbidaskasof-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Cross
      - Rates
      - Bid
      - Ask
      - As
      - Of
  /GetMutipleHistoricalCrossRates:
    get:
      summary: Get Mutiple Historical Cross Rates
      description: Returns multiple cross-rates as of a historical date.
      operationId: postGetmutiplehistoricalcrossrates
      x-api-path-slug: getmutiplehistoricalcrossrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Mutiple
      - Historical
      - Cross
      - Rates
  /GetAverageHistoricalCrossRates:
    get:
      summary: Get Average Historical Cross Rates
      description: This operation returns an array average daily historical cross-rates
        for a period.
      operationId: postGetaveragehistoricalcrossrates
      x-api-path-slug: getaveragehistoricalcrossrates-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Average
      - Historical
      - Cross
      - Rates
  /GetAverageHistoricalCrossRate:
    get:
      summary: Get Average Historical Cross Rate
      description: This operation returns an average daily historical cross-rates
        for a period.
      operationId: postGetaveragehistoricalcrossrate
      x-api-path-slug: getaveragehistoricalcrossrate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Average
      - Historical
      - Cross
      - Rate
  /GetHistoricalMonthlyCrossRatesRange:
    get:
      summary: Get Historical Monthly Cross Rates Range
      description: This operation returns a complete range of stock quotes for a currency
        pair.
      operationId: postGethistoricalmonthlycrossratesrange
      x-api-path-slug: gethistoricalmonthlycrossratesrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Monthly
      - Cross
      - Rates
      - Range
  /GetHistoricalTicks:
    get:
      summary: Get Historical Ticks
      description: Returns a historical range of ticks for a security.
      operationId: postGethistoricalticks
      x-api-path-slug: gethistoricalticks-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Ticks
  /GetHistoricalHighLow:
    get:
      summary: Get Historical High Low
      description: Returns the high and the low ticks for a historical time range.
      operationId: postGethistoricalhighlow
      x-api-path-slug: gethistoricalhighlow-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - High
      - Low
  /GetHistoricalFutureStrip:
    get:
      summary: Get Historical Future Strip
      description: Returns a future strip for a commodity.
      operationId: postGethistoricalfuturestrip
      x-api-path-slug: gethistoricalfuturestrip-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Future
      - Strip
  /GetHistoricalSwapStrip:
    get:
      summary: Get Historical Swap Strip
      description: Returns a future strip for a commodity.
      operationId: postGethistoricalswapstrip
      x-api-path-slug: gethistoricalswapstrip-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Swap
      - Strip
  /GetHistoricalFuture:
    get:
      summary: Get Historical Future
      description: Returns a historical quote for a future contract.
      operationId: postGethistoricalfuture
      x-api-path-slug: gethistoricalfuture-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Future
  /GetHistoricalFutures:
    get:
      summary: Get Historical Futures
      description: Returns historical quotes for multiple future contracts.
      operationId: postGethistoricalfutures
      x-api-path-slug: gethistoricalfutures-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Futures
  /GetAllHistoricalFuturesWithStatus:
    get:
      summary: Get All Historical Futures With Status
      description: Returns historical quotes for all contracts for a commodity as
        of a specific date including status information.
      operationId: postGetallhistoricalfutureswithstatus
      x-api-path-slug: getallhistoricalfutureswithstatus-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Futures
      - With
      - Status
  /GetAllHistoricalFutures:
    get:
      summary: Get All Historical Futures
      description: Returns historical quotes for all contracts for a commodity as
        of a specific date.
      operationId: postGetallhistoricalfutures
      x-api-path-slug: getallhistoricalfutures-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Futures
  /GetHistoricalFutureRange:
    get:
      summary: Get Historical Future Range
      description: Returns a range of historical quotes for a future contract.
      operationId: postGethistoricalfuturerange
      x-api-path-slug: gethistoricalfuturerange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Future
      - Range
  /GetHistoricalSwap:
    get:
      summary: Get Historical Swap
      description: Returns a historical quote for a future swap.
      operationId: postGethistoricalswap
      x-api-path-slug: gethistoricalswap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Swap
  /GetHistoricalSwapRange:
    get:
      summary: Get Historical Swap Range
      description: Returns a range of historical quotes for a future swap.
      operationId: postGethistoricalswaprange
      x-api-path-slug: gethistoricalswaprange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Swap
      - Range
  /GetHistoricalSwaps:
    get:
      summary: Get Historical Swaps
      description: Returns historical quotes for multiple future swaps.
      operationId: postGethistoricalswaps
      x-api-path-slug: gethistoricalswaps-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Swaps
  /GetAllHistoricalSwaps:
    get:
      summary: Get All Historical Swaps
      description: Returns historical quotes for all contracts for a commodity swap
        as of a specific date.
      operationId: postGetallhistoricalswaps
      x-api-path-slug: getallhistoricalswaps-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Swaps
  /GetHistoricalCommodityRange:
    get:
      summary: Get Historical Commodity Range
      description: Returns a range of historical quotes for a future contract.
      operationId: postGethistoricalcommodityrange
      x-api-path-slug: gethistoricalcommodityrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Commodity
      - Range
  /GetHistoricalCommodityMonthlyRange:
    get:
      summary: Get Historical Commodity Monthly Range
      description: Returns a range of historical quotes for a future contract.
      operationId: postGethistoricalcommoditymonthlyrange
      x-api-path-slug: gethistoricalcommoditymonthlyrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Commodity
      - Monthly
      - Range
  /GetHistoricalSpotRange:
    get:
      summary: Get Historical Spot Range
      description: Returns a range of commodity spot prices for a commodity.
      operationId: postGethistoricalspotrange
      x-api-path-slug: gethistoricalspotrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Spot
      - Range
  /GetHistoricalSpotMonthlyRange:
    get:
      summary: Get Historical Spot Monthly Range
      description: Returns a range of commodity spot prices for a commodity.
      operationId: postGethistoricalspotmonthlyrange
      x-api-path-slug: gethistoricalspotmonthlyrange-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Spot
      - Monthly
      - Range
  /GetHistoricalTicksAsOfDate:
    get:
      summary: Get Historical Ticks As Of Date
      description: Returns a historical range of ticks for a security.
      operationId: postGethistoricalticksasofdate
      x-api-path-slug: gethistoricalticksasofdate-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Ticks
      - As
      - Of
      - Date
  'Historical, Future, ':
    get:
      summary: Get Historical Future Chart
      description: Get a standard historical price chart for a future contract.
      operationId: postGethistoricalfuturechart
      x-api-path-slug: historical-future-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Future
      - Chart
  Historical, Future, , Binary:
    get:
      summary: Get Historical Future Chart Binary
      description: Get a standard historical price chart for a future contract in
        binary format.
      operationId: postGethistoricalfuturechartbinary
      x-api-path-slug: historical-future--binary-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Future
      - Chart
      - Binary
  Historical, Future, , Custom:
    get:
      summary: Get Historical Future Chart Custom
      description: Get a custom historical chart for a future contract in binary format.
      operationId: postGethistoricalfuturechartcustom
      x-api-path-slug: historical-future--custom-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Future
      - Chart
      - Custom
  Historical, Future, , Custom, Binary:
    get:
      summary: Get Historical Future Chart Custom Binary
      description: Draw a custom historical chart for a future contract.
      operationId: postGethistoricalfuturechartcustombinary
      x-api-path-slug: historical-future--custom-binary-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Future
      - Chart
      - Custom
      - Binary
  'Historical, Commodity, ':
    get:
      summary: Get Historical Commodity Chart
      description: Get a historical chart for a commodity.
      operationId: postGethistoricalcommoditychart
      x-api-path-slug: historical-commodity-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Historical
      - Commodity
      - Chart
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---