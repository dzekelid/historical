---
swagger: "2.0"
x-collection-name: nFusion Solutions
x-complete: 0
info:
  title: nFusion API Get historical benchmark prices for requested metals
  description: "Historical OHLC data for the specified period and interval size\r\n\r\nThe
    combination of the interval parameter and start and end dates can result in results\r\nbeing
    truncated to conform to result size limits. See comments on interval parameter
    for details on valid interval values.\r\n\r\nThe historicalfx flag is used to
    determine whether to apply today's fx rates to a historical period, or to apply
    the historical rates from that same time frame."
  contact:
    name: nFusion Solutions
    url: https://nfusionsolutions.com/contact
    email: support@nfusionsolutions.com
  version: 1.0.0
host: api.nfusionsolutions.biz
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v{version}/Currencies/history:
    get:
      summary: Get historical prices for requested currency pairs
      description: "Historical OHLC data for the specified period and interval size\r\n\r\nThe
        combination of the interval parameter and start and end dates can result in
        results\r\nbeing truncated to conform to result size limits. See comments
        on interval parameter for details on valid interval values."
      operationId: ApiV{versionCurrenciesHistoryGet
      x-api-path-slug: apivversioncurrencieshistory-get
      parameters:
      - in: query
        name: end
        description: end date of time period
      - in: query
        name: format
        description: to override content negotiation specify a value of json or xml
      - in: query
        name: interval
        description: aggregation interval
      - in: query
        name: pairs
        description: comma separated list of currency pairs
      - in: query
        name: start
        description: start date of time period
      - in: query
        name: token
        description: auth token
      - in: path
        name: version
        description: The requested API version
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Pricesrequested
      - Currency
      - Pairs
  /api/v{version}/Metals/spot/history:
    get:
      summary: Get historical Spot prices for requested metals
      description: "Historical OHLC data for the specified period and interval size\r\n\r\nThe
        combination of the interval parameter and start and end dates can result in
        results\r\nbeing truncated to conform to result size limits. See comments
        on interval parameter for details on valid interval values.\r\n\r\nThe historicalfx
        flag is used to determine whether to apply today's fx rates to a historical
        period, or to apply the historical rates from that same time frame."
      operationId: ApiV{versionMetalsSpotHistoryGet
      x-api-path-slug: apivversionmetalsspothistory-get
      parameters:
      - in: query
        name: currency
        description: comma separated list of conversion currencies, defaults to USD
      - in: query
        name: end
        description: end date of time period
      - in: query
        name: format
        description: to override content negotiation specify a value of json or xml
      - in: query
        name: historicalfx
        description: if true use historical currency rates otherwise current currency
          rates
      - in: query
        name: interval
        description: aggregation interval
      - in: query
        name: metals
        description: comma separated list of metals
      - in: query
        name: start
        description: start date of time period
      - in: query
        name: token
        description: auth token
      - in: query
        name: unitofmeasure
        description: unit of meaure, defaults to troy ounces
      - in: path
        name: version
        description: The requested API version
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Spot
      - Pricesrequested
      - Metals
  /api/v{version}/Metals/spot/ratio/history:
    get:
      summary: Get historical Spot Ratio prices for requested metals
      description: "Historical data for the specified period and interval size\r\n\r\nThe
        combination of the interval parameter and start and end dates can result in
        results\r\nbeing truncated to conform to result size limits. See comments
        on interval parameter for details on valid interval values."
      operationId: ApiV{versionMetalsSpotRatioHistoryGet
      x-api-path-slug: apivversionmetalsspotratiohistory-get
      parameters:
      - in: query
        name: end
        description: end date of time period
      - in: query
        name: format
        description: to override content negotiation specify a value of json or xml
      - in: query
        name: interval
        description: aggregation interval
      - in: query
        name: pairs
        description: comma separated list of metals
      - in: query
        name: start
        description: start date of time period
      - in: query
        name: token
        description: auth token
      - in: path
        name: version
        description: The requested API version
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Spot
      - Ratio
      - Pricesrequested
      - Metals
  /api/v{version}/Metals/benchmark/history:
    get:
      summary: Get historical benchmark prices for requested metals
      description: "Historical OHLC data for the specified period and interval size\r\n\r\nThe
        combination of the interval parameter and start and end dates can result in
        results\r\nbeing truncated to conform to result size limits. See comments
        on interval parameter for details on valid interval values.\r\n\r\nThe historicalfx
        flag is used to determine whether to apply today's fx rates to a historical
        period, or to apply the historical rates from that same time frame."
      operationId: ApiV{versionMetalsBenchmarkHistoryGet
      x-api-path-slug: apivversionmetalsbenchmarkhistory-get
      parameters:
      - in: query
        name: currency
        description: comma separated list of conversion currencies, defaults to USD
      - in: query
        name: end
        description: end date of time period
      - in: query
        name: format
        description: to override content negotiation specify a value of json or xml
      - in: query
        name: historicalfx
        description: if true use historical currency rates otherwise current currency
          rates
      - in: query
        name: interval
        description: aggregation interval
      - in: query
        name: metals
        description: comma separated list of metals
      - in: query
        name: start
        description: start date of time period
      - in: query
        name: token
        description: auth token
      - in: query
        name: unitofmeasure
        description: unit of meaure, defaults to troy ounces
      - in: path
        name: version
        description: The requested API version
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Benchmark
      - Pricesrequested
      - Metals
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