---
swagger: "2.0"
x-collection-name: nFusion Solutions
x-complete: 1
info:
  title: nFusion Solutions Market Data API v1
  description: nfusion-solutions-provides-rest-and-streaming-apis-that-deliver-enterprisegrade-financial-data--data-sets-include-realtime-and-historical-pricing-for-spot-prices-of-precious-metals-such-as-gold-silver-platinum-and-palladium-exchange-rates-for-major-currency-pairs-exchange-rates-for-crypto-currencies-such-as-btc-eth-and-ltc--all-api-access-requires-authentication--in-order-to-be-issued-access-credentials-you-must-first-enter-into-a-service-agreement-with-nfusion-solutions-and-acquire-a-commercial-license--for-information-on-how-to-obtain-a-licence-contact-salesnfusionsolutions-com-
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
  /api/v{version}/Metals/spot/performance/annual:
    get:
      summary: Get Historical Annual Performance for requested metals
      description: Get historical annual performance for requested metals.
      operationId: ApiV{versionMetalsSpotPerformanceAnnualGet
      x-api-path-slug: apivversionmetalsspotperformanceannual-get
      parameters:
      - in: query
        name: currency
        description: comma separated list of conversion currencies, defaults to USD
      - in: query
        name: format
        description: to override content negotiation specify a value of json or xml
      - in: query
        name: metals
        description: comma separated list of metals
      - in: query
        name: token
        description: auth token
      - in: query
        name: unitofmeasure
        description: unit of meaure, defaults to troy ounces
      - in: path
        name: version
        description: The requested API version
      - in: query
        name: years
        description: Number of years of history to return
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Annual
      - Performancerequested
      - Metals
  /api/v{version}/Metals/spot/performance:
    get:
      summary: Get Historical Performance for requested metals
      description: Get historical performance for requested metals.
      operationId: ApiV{versionMetalsSpotPerformanceGet
      x-api-path-slug: apivversionmetalsspotperformance-get
      parameters:
      - in: query
        name: currency
        description: comma separated list of conversion currencies, defaults to USD
      - in: query
        name: format
        description: to override content negotiation specify a value of json or xml
      - in: query
        name: metals
        description: comma separated list of metals
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
      - Performancerequested
      - Metals
---