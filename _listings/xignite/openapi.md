---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /GetHistoricalDailyVWAP:
    get:
      summary: Get Historical Daily VWAP
      description: Returns historical daily VWAP information for a date range
      operationId: GetHistoricalDailyVWAP
      x-api-path-slug: gethistoricaldailyvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Daily
      - VWAP
  /GetHistoricalVWAP:
    get:
      summary: Get Historical VWAP
      description: Returns historical VWAP information for a date range
      operationId: GetHistoricalVWAP
      x-api-path-slug: gethistoricalvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - VWAP
  /GetHistoricalMonthlyVWAP:
    get:
      summary: Get Historical Monthly VWAP
      description: Returns historical monthly VWAP information for a date range.
      operationId: GetHistoricalMonthlyVWAP
      x-api-path-slug: gethistoricalmonthlyvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Monthly
      - VWAP
  /GetHistoricalWeeklyVWAP:
    get:
      summary: Get Historical Weekly VWAP
      description: Returns historical weekly VWAP information for a date range.
      operationId: GetHistoricalWeeklyVWAP
      x-api-path-slug: gethistoricalweeklyvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Weekly
      - VWAP
  /GetHistoricalPeriodVWAP:
    get:
      summary: Get Historical Period VWAP
      description: Returns historical VWAP information for a date range.
      operationId: GetHistoricalPeriodVWAP
      x-api-path-slug: gethistoricalperiodvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Period
      - VWAP
  /GetHistoricalIntradayVWAP:
    get:
      summary: Get Historical Intraday VWAP
      description: Returns a historical intraday VWAP for a security based on the
        trades performed in a time range.
      operationId: GetHistoricalIntradayVWAP
      x-api-path-slug: gethistoricalintradayvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Historical
      - Intraday
      - VWAP
  /GetCorporateHistoricalVWAP:
    get:
      summary: Get Corporate Historical VWAP
      description: Returns a corporate intraday VWAP for a security based on the trades
        performed in a time range.
      operationId: GetCorporateHistoricalVWAP
      x-api-path-slug: getcorporatehistoricalvwap-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Corporate
      - Historical
      - VWAP
---