swagger: "2.0"
x-collection-name: HitBTC
x-complete: 1
info:
  title: HitBTC API
  description: create-api-keys-in-your-profile-httpshitbtc-comsettingsapikeys-and-use-public-api-key-as-username-and-secret-as-password-to-authorize-
  version: 1.0.0
basePath: /api/2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /history/trades:
    get:
      summary: Get Historical Trades
      description: Get historical trades.
      operationId: getHistoryTrades
      x-api-path-slug: historytrades-get
      parameters:
      - in: query
        name: by
        description: Filter field
      - in: query
        name: from
        description: If filter by timestamp, then datetime in iso format or timestamp
          in millisecond otherwise trade id
      - in: query
        name: limit
      - in: query
        name: offset
      - in: query
        name: sort
        description: Sort direction
      - in: query
        name: symbol
      - in: query
        name: till
        description: If filter by timestamp, then datetime in iso format or timestamp
          in millisecond otherwise trade id
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Trades
  /history/order:
    get:
      summary: Get Historical Orders
      description: Get historical orders.
      operationId: getHistoryOrder
      x-api-path-slug: historyorder-get
      parameters:
      - in: query
        name: clientOrderId
      - in: query
        name: from
        description: Datetime in iso format or timestamp in millisecond
      - in: query
        name: limit
      - in: query
        name: offset
      - in: query
        name: symbol
      - in: query
        name: till
        description: Datetime in iso format or timestamp in millisecond
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Orders
  /history/order/{id}/trades:
    get:
      summary: Get Historical Trades By Specified Order
      description: Get historical trades by specified order.
      operationId: getHistoryOrderTrades
      x-api-path-slug: historyorderidtrades-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Trades
      - By
      - Specified
      - Order