---
swagger: "2.0"
x-collection-name: Barchart
x-complete: 0
info:
  title: Barchart API Get Close Price
  description: Get the close price for given instruments for the given date.
  version: 1.0.0
host: marketdata.websol.barchart.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /getClosePrice.json:
    get:
      summary: Get Close Price
      description: Get the close price for given instruments for the given date.
      operationId: getClosePrice
      x-api-path-slug: getcloseprice-json-get
      parameters:
      - in: query
        name: symbols
        description: A symbol or code that identifies a financial instrument
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Stocks
      - Price
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