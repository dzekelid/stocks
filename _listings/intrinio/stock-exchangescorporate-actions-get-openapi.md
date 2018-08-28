---
swagger: "2.0"
x-collection-name: Intrinio
x-complete: 0
info:
  title: Intrinio API Stock Exchange Corporate Actions
  description: 'Returns all corporate actions for all securities listed on a specified
    stock exchange.  A subscription to the EDI Corporate Actions Data Feed for a specific
    country will permit access to all stock exchanges in that country (ie, US includes
    NASDAQ, NYSE, BATS). Events 45+ types of corporate actions such as: Announcements
    and Annual Shareholder Meetings, Ex-date, Dividend pay date, Splits, Buy Backs,
    M&amp;A and Takeovers, Bankruptcies and much more'
  version: 1.0.0
host: api.intrinio.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /stock_exchanges:
    get:
      summary: Stock Exchange Master
      description: Returns stock exchange list and information for all stock exchanges
        covered by Intrinio.
      operationId: stock-exchange-master
      x-api-path-slug: stock-exchanges-get
      parameters:
      - in: query
        name: page_number
        description: an integer greater than or equal to 1 for specifying the page
          number for the return values
        type: string
      - in: query
        name: page_size
        description: an integer greater than 1 for specifying the number of results
          on each page
        type: string
      - in: query
        name: query
        description: a string query search of stock exchange name or MIC with the
          returned results being the relevant stock exchanges in compacted list format
        type: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Stock Exchanges
  /stock_exchanges/corporate_actions:
    get:
      summary: Stock Exchange Corporate Actions
      description: 'Returns all corporate actions for all securities listed on a specified
        stock exchange.  A subscription to the EDI Corporate Actions Data Feed for
        a specific country will permit access to all stock exchanges in that country
        (ie, US includes NASDAQ, NYSE, BATS). Events 45+ types of corporate actions
        such as: Announcements and Annual Shareholder Meetings, Ex-date, Dividend
        pay date, Splits, Buy Backs, M&amp;A and Takeovers, Bankruptcies and much
        more'
      operationId: stock-exchange-corporate-actions
      x-api-path-slug: stock-exchangescorporate-actions-get
      parameters:
      - in: query
        name: identifier
        description: 'the stock market ticker symbol associated with the companies
          common stock securities or the stock market index:'
        type: string
      - in: query
        name: page_number
        description: an integer greater than or equal to 1 for specifying the page
          number for the return values
        type: string
      - in: query
        name: page_size
        description: an integer greater than 1 for specifying the number of results
          on each page
        type: string
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Stock Exchanges
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