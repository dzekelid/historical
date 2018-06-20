---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 0
info:
  title: Xignite Global Indices Historical Get Historical Index Value
  description: Get historical index value.
  version: 1.0.0
host: globalindiceshistorical.xignite.com
basePath: xglobalindiceshistorical.json/XigniteGlobalIndicesHistorical
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetHistoricalIndexValues:
    get:
      summary: Get Historical Index Values
      description: Get historical index values.
      operationId: GetHistoricalIndexValues
      x-api-path-slug: gethistoricalindexvalues-get
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
      - Index
      - Values
  /GetHistoricalIndicesValue:
    get:
      summary: Get Historical Indices Value
      description: Get historical indices value.
      operationId: GetHistoricalIndicesValue
      x-api-path-slug: gethistoricalindicesvalue-get
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
      - Indices
      - Value
  /GetHistoricalIndexValue:
    get:
      summary: Get Historical Index Value
      description: Get historical index value.
      operationId: GetHistoricalIndexValue
      x-api-path-slug: gethistoricalindexvalue-get
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
      - Index
      - Value
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