---
swagger: "2.0"
x-collection-name: LinkedIn
x-complete: 1
info:
  title: LinkedIn
  description: bring-user-profiles-and-professional-networks-to-your-apps-
  version: 1.0.0
host: api.linkedin.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /companies/{id}/historical-follow-statistics:
    get:
      summary: Get Companies Historical Follow Statistics
      description: Get companies  historical follow statistics
      operationId: getCompaniesHistoricalFollowStatistics
      x-api-path-slug: companiesidhistoricalfollowstatistics-get
      parameters:
      - in: query
        name: format
        description: The message format
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Companies
      - ""
      - Historical
      - Follow
      - Statistics
  /companies/{id}/historical-status-update-statistics:
    get:
      summary: Get Companies Historical Status Update Statistics
      description: Get companies  historical status update statistics
      operationId: getCompaniesHistoricalStatusUpdateStatistics
      x-api-path-slug: companiesidhistoricalstatusupdatestatistics-get
      parameters:
      - in: query
        name: format
        description: The message format
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Companies
      - ""
      - Historical
      - Status
      - Update
      - Statistics
---