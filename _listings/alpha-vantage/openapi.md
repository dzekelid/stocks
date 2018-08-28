swagger: "2.0"
x-collection-name: Alpha Vantage
x-complete: 1
info:
  title: Alpha Vantage
  description: alpha-vantage-apis-are-grouped-into-four-categories-1-stock-time-series-data-2-physical-and-digitalcrypto-currencies-e-g--bitcoin-3-stock-technical-indicators-and-4-sector-performances--all-apis-are-realtime-the-latest-data-points-are-derived-from-the-current-trading-day--
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