---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Money Markets Get Historical Swap Rate Extended Range
  description: Returns historical Swap rate range
  version: 1.0.0
host: www.xignite.com
basePath: xMoneyMarkets.json/XigniteMoneyMarkets
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetHistoricalSwaption:
    get:
      summary: Get Historical Swaption
      description: Returns a Swaption as of a historical date
      operationId: postGethistoricalswaption
      x-api-path-slug: gethistoricalswaption-get
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
      - Swaption
  /GetHistoricalSwaptionFamily:
    get:
      summary: Get Historical Swaption Family
      description: Returns a Swaption rate Family
      operationId: postGethistoricalswaptionfamily
      x-api-path-slug: gethistoricalswaptionfamily-get
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
      - Swaption
      - Family
  /GetHistoricalSwapRate:
    get:
      summary: Get Historical Swap Rate
      description: Returns a Swap rate as of a historical date
      operationId: postGethistoricalswaprate
      x-api-path-slug: gethistoricalswaprate-get
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
      - Rate
  /GetHistoricalSwapRateRange:
    get:
      summary: Get Historical Swap Rate Range
      description: Returns a Swap rate as of a historical date
      operationId: postGethistoricalswapraterange
      x-api-path-slug: gethistoricalswapraterange-get
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
      - Rate
      - Range
  /GetHistoricalSwapRateExtended:
    get:
      summary: Get Historical Swap Rate Extended
      description: Returns historical swap rate
      operationId: postGethistoricalswaprateextended
      x-api-path-slug: gethistoricalswaprateextended-get
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
      - Rate
      - Extended
  /GetHistoricalSwapRateExtendedRange:
    get:
      summary: Get Historical Swap Rate Extended Range
      description: Returns historical Swap rate range
      operationId: postGethistoricalswaprateextendedrange
      x-api-path-slug: gethistoricalswaprateextendedrange-get
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
      - Rate
      - Extended
      - Range
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