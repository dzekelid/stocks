---
swagger: "2.0"
x-collection-name: Alpha Vantage
x-complete: 0
info:
  title: Alpha Vantage Batch Stock Quotes
  description: The batch stock quotes API enables the querying of multiple stock quotes
    with a single API request, updated realtime. It may serve as a lightweight alternative
    to our core stock time series APIs above (which have richer content but are symbol-specific).
  version: 1.0.0
host: www.alphavantage.co
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /query?function=BATCH_STOCK_QUOTES:
    get:
      summary: Batch Stock Quotes
      description: The batch stock quotes API enables the querying of multiple stock
        quotes with a single API request, updated realtime. It may serve as a lightweight
        alternative to our core stock time series APIs above (which have richer content
        but are symbol-specific).
      operationId: getBatchStockQuotes
      x-api-path-slug: queryfunctionbatch-stock-quotes-get
      parameters:
      - in: query
        name: symbols
        description: Up to 100 stock symbols seperated by comma
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Time Series
      - Stock Quotes
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