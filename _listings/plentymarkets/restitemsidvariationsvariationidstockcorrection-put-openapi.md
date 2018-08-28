---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets Correct stock
  description: Corrects stock. The item ID and the variation ID must be specified.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rest/items/{id}/variations/{variationId}/stock:
    get:
      summary: List stock of a variation per warehouse
      description: Lists stock of a variation per warehouse. The ID of the item and
        the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationStock
      x-api-path-slug: restitemsidvariationsvariationidstock-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: id
      - in: query
        name: itemId
        description: The ID of the item
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - Of
      - Variation
      - Per
      - Warehouse
  /rest/items/{id}/variations/{variationId}/stock/bookIncomingItems:
    put:
      summary: Book incoming stock
      description: Books incoming stock for a variation. The incoming stock will be
        added to the existing stock. The ID of the item and the ID of the variation
        must be specified.
      operationId: putRestItemsVariationsVariationStockBookincomingitems
      x-api-path-slug: restitemsidvariationsvariationidstockbookincomingitems-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/stock/bookIncomingItems
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: query
        name: itemId
        description: The ID of the item
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Book
      - Incoming
      - Stock
  /rest/items/{id}/variations/{variationId}/stock/correction:
    put:
      summary: Correct stock
      description: Corrects stock. The item ID and the variation ID must be specified.
      operationId: putRestItemsVariationsVariationStockCorrection
      x-api-path-slug: restitemsidvariationsvariationidstockcorrection-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/stock/correction
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: query
        name: itemId
        description: The ID of the item
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Correct
      - Stock
  /rest/items/{id}/variations/{variationId}/stock/movements:
    get:
      summary: List stock movements
      description: |-
        Lists stock movements for a variation. The ID of the item and the ID of the variation must be specified. To get movements older than 3 months, set the 'year' parameter.
        NOTE: You can either get archive entries or non-archive entries. You can not get entries for the current year that are younger and older than 3 months with one request. You need separate requests to get entries older and younger than 3 months. To get all entries younger than 3 month you do not need to specify a year or any createdAt parameter.
      operationId: getRestItemsVariationsVariationStockMovements
      x-api-path-slug: restitemsidvariationsvariationidstockmovements-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: createdAtFrom
        description: Get entries with createdAt date after this date
      - in: query
        name: createdAtTo
        description: Get entries with createdAt date before this date
      - in: path
        name: id
      - in: query
        name: itemId
        description: The ID of the item
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: path
        name: variationId
      - in: query
        name: warehouseId
        description: The ID of the warehouse
      - in: query
        name: year
        description: Get entries from the archive for the given year
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - Movements
  /rest/items/{id}/variations/{variationId}/stock/redistribute:
    put:
      summary: Redistribute stock
      description: Redistributes the stock of one storage location among one or more
        storage locations. The item ID and the variation ID need to be specified.
      operationId: putRestItemsVariationsVariationStockRedistribute
      x-api-path-slug: restitemsidvariationsvariationidstockredistribute-put
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/stock/redistribute
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: query
        name: itemId
        description: The ID of the item
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Redistribute
      - Stock
  /rest/items/{id}/variations/{variationId}/stock/storageLocations:
    get:
      summary: List stock of a variation per storage locations
      description: Lists stock of a variation per storage location. The ID of the
        item and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationStockStoragelocations
      x-api-path-slug: restitemsidvariationsvariationidstockstoragelocations-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: id
      - in: query
        name: itemId
        description: The ID of the item
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - Of
      - Variation
      - Per
      - Storage
      - Locations
  /rest/listings/stock_dependence_types:
    get:
      summary: List listing stock dependence types
      description: Lists listing stock dependence types.
      operationId: getRestListingsStockDependenceTypes
      x-api-path-slug: restlistingsstock-dependence-types-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Stock
      - Dependence
      - Types
  /rest/listings/stock_dependence_types/{id}:
    get:
      summary: Get a listing stock dependence type
      description: Gets a listing stock dependence type by given ID.
      operationId: getRestListingsStockDependenceTypes
      x-api-path-slug: restlistingsstock-dependence-typesid-get
      parameters:
      - in: path
        name: id
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - Listing
      - Stock
      - Dependence
      - Type
  /rest/orders/{orderId}/outgoing_stocks:
    delete:
      summary: Revert outgoing stock
      description: Reverts the booking of order items of an order. The ID of the order
        must be specified.
      operationId: deleteRestOrdersOrderOutgoingStocks
      x-api-path-slug: restordersorderidoutgoing-stocks-delete
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - Revert
      - Outgoing
      - Stock
  /rest/stockmanagement/stock:
    get:
      summary: List stock
      description: Lists stock of all warehouses.
      operationId: getRestStockmanagementStock
      x-api-path-slug: reststockmanagementstock-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to stock that were last
          updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to stock that were last
          updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to stock with a variation
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
  /rest/stockmanagement/stock/redistribute:
    put:
      summary: Redistribute stock
      description: Redistributes stock of one storage location among one or more storage
        locations.
      operationId: putRestStockmanagementStockRedistribute
      x-api-path-slug: reststockmanagementstockredistribute-put
      parameters:
      - in: body
        name: /rest/stockmanagement/stock/redistribute
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Redistribute
      - Stock
  /rest/stockmanagement/stock/types/{type}:
    get:
      summary: List stock by warehouse type
      description: Lists stock for all warehouses of the same warehouse type. The
        name of the type must be specified. Currently the only type available is 'sales'.
      operationId: getRestStockmanagementStockTypesType
      x-api-path-slug: reststockmanagementstocktypestype-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: path
        name: type
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to stock that were last
          updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to stock that were last
          updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to stock with a variation
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - By
      - Warehouse
      - Type
  /rest/stockmanagement/warehouses/{warehouseId}/stock:
    get:
      summary: List stock by warehouse
      description: Lists stock for a warehouse. The ID of the warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseStock
      x-api-path-slug: reststockmanagementwarehouseswarehouseidstock-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to stock that were last
          updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to stock that were last
          updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to stock with a variation
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - By
      - Warehouse
  /rest/stockmanagement/warehouses/{warehouseId}/stock/bookIncomingItems:
    put:
      summary: Book incoming stock
      description: Books incoming stock for multiple variations. The incoming stock
        will be added to the existing stock. The ID of the warehouse must be specified.
      operationId: putRestStockmanagementWarehousesWarehouseStockBookincomingitems
      x-api-path-slug: reststockmanagementwarehouseswarehouseidstockbookincomingitems-put
      parameters:
      - in: body
        name: /rest/stockmanagement/warehouses/{warehouseId}/stock/bookIncomingItems
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - Book
      - Incoming
      - Stock
  /rest/stockmanagement/warehouses/{warehouseId}/stock/correction:
    put:
      summary: Correct stock
      description: Corrects stock. The ID of the warehouse must be specified.
      operationId: putRestStockmanagementWarehousesWarehouseStockCorrection
      x-api-path-slug: reststockmanagementwarehouseswarehouseidstockcorrection-put
      parameters:
      - in: body
        name: /rest/stockmanagement/warehouses/{warehouseId}/stock/correction
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - Correct
      - Stock
  /rest/stockmanagement/warehouses/{warehouseId}/stock/movements:
    get:
      summary: List stock movements
      description: |-
        Lists stock movements for a warehouse. The ID of the warehouse must be specified. To get movements older than 3 months, set the 'year' parameter.
        NOTE: You can either get archive entries or non-archive entries. You can not get entries for the current year that are younger and older than 3 months with one request. You need separate requests to get entries older and younger than 3 months. To get all entries younger than 3 month you do not need to specify a year or any createdAt parameter.
      operationId: getRestStockmanagementWarehousesWarehouseStockMovements
      x-api-path-slug: reststockmanagementwarehouseswarehouseidstockmovements-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: createdAtFrom
        description: Get entries with createdAt date after this date
      - in: query
        name: createdAtTo
        description: Get entries with createdAt date before this date
      - in: query
        name: itemId
        description: The ID of the item
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: query
        name: variationId
        description: The ID of the variation
      - in: path
        name: warehouseId
      - in: query
        name: year
        description: Get entries from the archive for the given year
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - Movements
  /rest/stockmanagement/warehouses/{warehouseId}/stock/storageLocations:
    get:
      summary: List stock of a warehouse per storage location
      description: Lists stock of a warehouse for each variation and storage location.
        The stock will only be listed if the stock is positive. Negative stock will
        not be listed. The ID of the warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseStockStoragelocations
      x-api-path-slug: reststockmanagementwarehouseswarehouseidstockstoragelocations-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: query
        name: storageLocationId
        description: Filter that restricts the search result to stock of a storage
          location
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to stock that were last
          updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to stock that were last
          updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to stock with a variation
      - in: path
        name: warehouseId
      - in: query
        name: with
        description: Load additional relations for a StockStorageLocation
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - Of
      - Warehouse
      - Per
      - Storage
      - Location
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