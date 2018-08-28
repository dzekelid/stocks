{
  "info": {
    "name": "Plentymarkets List stock by warehouse type",
    "_postman_id": "9f81bcd0-b4fc-4ae5-bcfa-fe019f04b0d0",
    "description": "Lists stock for all warehouses of the same warehouse type. The name of the type must be specified. Currently the only type available is 'sales'.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Address",
      "item": [
        {
          "id": "c8037daa-c297-414b-8821-61bc3fc52b81",
          "name": "postRestAccountsAddressesWarehouseRelations",
          "request": {
            "url": "http://example.com/rest/accounts/addresses/warehouse_relations",
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Create an address warehouse relation."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4f43e550-65ab-43a3-9f87-204c6a206365"
            }
          ]
        },
        {
          "id": "7d1c3cf2-1904-4b09-b5de-bc8df9ad3b6b",
          "name": "putRestAccountsAddressesWarehouseRelationsRelation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/addresses/warehouse_relations/:relationId"
              ],
              "variable": [
                {
                  "id": "relationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Updates an address warehouse relation. The ID of the relation must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e4cbca1-b535-4815-9776-6844a73e105c"
            }
          ]
        },
        {
          "id": "5ffdd0cc-d034-4cef-81e4-deefb179ab70",
          "name": "deleteRestAccountsAddressesWarehouseRelationsRelation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/accounts/addresses/warehouse_relations/:relationId"
              ],
              "variable": [
                {
                  "id": "relationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an address warehouse relation. The ID of the relation must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "30aa1868-7a82-4832-986f-361ed31f7ef5"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "af018148-61d7-4bfb-a83a-6970184bbf7e",
          "name": "getRestItemsVariationsVariationStock",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/stock"
              ],
              "query": [
                {
                  "key": "columns",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "itemId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists stock of a variation per warehouse. The ID of the item and the ID of the variation must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cc2b4dcb-4006-4bc8-bb27-4b80be529c89"
            }
          ]
        },
        {
          "id": "3874677f-73c8-44ff-aa13-2c906c5fda59",
          "name": "getRestStockmanagementStockTypesType",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/stockmanagement/stock/types/:type"
              ],
              "query": [
                {
                  "key": "columns",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "itemsPerPage",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "page",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "updatedAtFrom",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "updatedAtTo",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "variationId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "type",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Lists stock for all warehouses of the same warehouse type. The name of the type must be specified. Currently the only type available is 'sales'."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "027bb592-90cd-4529-bef5-bdb375abd3a8"
            }
          ]
        }
      ]
    },
    {
      "name": "Link",
      "item": [
        {
          "id": "b79f2e13-6955-4079-88de-b7cff9e9dcfb",
          "name": "postRestItemsVariationsVariationVariationWarehouses",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_warehouses"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Creates a link between a variation and a warehouse and adds warehouse data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9f317ba7-7c7c-427e-9c7f-380fa280351a"
            }
          ]
        },
        {
          "id": "c8944768-5075-4fa2-bd07-b020b048f390",
          "name": "deleteRestItemsVariationsVariationVariationWarehousesWarehouse",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_warehouses/:warehouseId"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "warehouseId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the link between a warehouse and a variation. The ID of the variation and the ID of the warehouse must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a105c3a-ffb4-4aaf-9fc5-ba4f52bfdbec"
            }
          ]
        }
      ]
    },
    {
      "name": "Warehouse",
      "item": [
        {
          "id": "eee151ca-3502-419d-8b5a-8b6ea3c412aa",
          "name": "getRestItemsVariationsVariationVariationWarehousesWarehouse",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_warehouses/:warehouseId"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "warehouseId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Gets the data of a warehouse linked to a variation. The ID of the variation and the ID of the warehouse must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1e3c5b5c-ff31-4dcc-9d6a-4c91c1762dd9"
            }
          ]
        },
        {
          "id": "666979c3-428d-4e48-a4bf-aa1b6d7c7531",
          "name": "putRestItemsVariationsVariationVariationWarehousesWarehouse",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/items/:id/variations/:variationId/variation_warehouses/:warehouseId"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "variationId",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "warehouseId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Updates the data of a warehouse linked to a variation. The ID of the variation and the ID of the warehouse must be specified."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2bed70a4-18ff-4c81-8163-1c5df3b8c7a1"
            }
          ]
        }
      ]
    }
  ]
}