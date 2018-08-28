swagger: "2.0"
x-collection-name: Clover
x-complete: 1
info:
  title: ""
  version: 1.0.0
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
    post:
      summary: Update the stock of an inventory item
      description: Update the stock of an inventory item.
      operationId: UpdateItemStock
      x-api-path-slug: v3merchantsmiditem-stocksitemid-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
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
    delete:
      summary: Delete the stock of an inventory item
      description: Delete the stock of an inventory item.
      operationId: DeleteItemStock
      x-api-path-slug: v3merchantsmiditem-stocksitemid-delete
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