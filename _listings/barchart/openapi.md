swagger: "2.0"
x-collection-name: Barchart
x-complete: 1
info:
  title: Barchart API
  description: stock-futures-and-forex-quotes-and-historical-data-
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