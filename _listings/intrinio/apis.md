---
name: Intrinio
x-slug: intrinio
description: Intelligent Data, On Demand. The financial data platform for developers,
  investors, students, and educators, with over 200 feeds including real-time, intraday,
  EOD, and international financial data available via REST API, WebSocket, CSV, Excel,
  and Goo...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28077-intrinio.jpg
x-kinRank: "8"
x-alexaRank: "303229"
tags: Historical
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/historical/master/_listings/intrinio/apis.md
specificationVersion: "0.14"
apis:
- name: Intrinio API Historical Data
  x-api-slug: intrinio-api
  description: Returns the historical data for for a selected identifier (ticker symbol
    or index symbol) for a selected tag.  The complete list of tags available through
    this function are available here.  Income statement, cash flow statement, and
    ratios are returned as trailing twelve months values by default, but can be changed
    with the type parameter.  All other historical data points are returned as their
    value on a certain day based on filings reported as of that date.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28077-intrinio.jpg
  humanURL: https://intrinio.com
  baseURL: https://api.intrinio.com////historical_data
  tags: Market Data,Historical Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/historical/master/_listings/intrinio/historical-data-get-openapi.md
- name: Intrinio API Historical Prices
  x-api-slug: intrinio-api
  description: Returns the historical prices for the given option contract.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28077-intrinio.jpg
  humanURL: https://intrinio.com
  baseURL: https://api.intrinio.com////options/historical
  tags: Market Data,Options,Historical
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/historical/master/_listings/intrinio/optionshistorical-get-openapi.md
- name: Intrinio API
  x-api-slug: intrinio-api
  description: Intelligent Data, On Demand. The financial data platform for developers,
    investors, students, and educators, with over 200 feeds including real-time, intraday,
    EOD, and international financial data available via REST API, WebSocket, CSV,
    Excel, and Goo...
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28077-intrinio.jpg
  humanURL: https://intrinio.com
  baseURL: https://api.intrinio.com//
  tags: Historical
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/historical/master/_listings/intrinio/openapi.md
x-common:
- type: x-applications-showcase
  url: https://intrinio.com/marketplace/apps
- type: x-authentication
  url: http://docs.intrinio.com/#authentication
- type: x-blog
  url: http://blog.intrinio.com/
- type: x-blog-rss
  url: http://blog.intrinio.com/feed/
- type: x-code
  url: http://docs.intrinio.com/#sdks
- type: x-crunchbase
  url: https://crunchbase.com/organization/tribunat
- type: x-developer
  url: https://intrinio.com/we-love-developers
- type: x-documentation
  url: https://intrinio.com/marketplace/data
- type: x-email
  url: cfarley@intrinio.com
- type: x-email
  url: admin@intrinio.com
- type: x-email
  url: support@intrinio.com
- type: x-email
  url: acarpenter@intrinio.com
- type: x-login
  url: https://intrinio.com/login
- type: x-partners
  url: https://intrinio.com/partners
- type: x-press
  url: https://intrinio.com/press
- type: x-rate-limits
  url: http://docs.intrinio.com/#limits
- type: x-selfservice-registration
  url: https://intrinio.com/signup
- type: x-spreadsheets
  url: http://docs.intrinio.com/#spreadsheet-add-ins
- type: x-support
  url: https://intrinio.com/help
- type: x-tutorial
  url: https://intrinio.com/tutorial/web_api
- type: x-twitter
  url: https://twitter.com/intrinio
- type: x-website
  url: https://intrinio.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---