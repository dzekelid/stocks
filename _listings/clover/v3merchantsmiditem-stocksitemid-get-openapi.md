---
swagger: "2.0"
x-collection-name: Clover
x-complete: 0
info:
  title: Clover Get the stock of an inventory item
  version: 1.0.0
  description: Get the stock of an inventory item.
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/item_stocks:
    get:
      summary: Get the stock of all inventory items
      description: Get the stock of all inventory items.
      operationId: GetItemStocks
      x-api-path-slug: v3merchantsmiditem-stocks-get
      parameters:
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Stocks
  /v3/merchants/{mId}/item_stocks/{itemId}:
    get:
      summary: Get the stock of an inventory item
      description: Get the stock of an inventory item.
      operationId: GetItemStock
      x-api-path-slug: v3merchantsmiditem-stocksitemid-get
      parameters:
      - in: path
        name: itemId
        description: Item Id
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Item
      - Stocks
      - ItemId
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