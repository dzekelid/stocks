{
  "info": {
    "name": "Plentymarkets List stock of a variation per warehouse",
    "_postman_id": "4405e7e7-93b2-444f-8116-129bd473c5fa",
    "description": "Lists stock of a variation per warehouse. The ID of the item and the ID of the variation must be specified.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Address",
      "item": [
        {
          "id": "b8d3295d-fd08-497d-8595-3bd3c13b85d3",
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
              "id": "8035e209-49af-4ec7-876b-4bae1fa2ec2e"
            }
          ]
        },
        {
          "id": "c95cf4d7-18db-4ab3-9934-60e6fa542744",
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
              "id": "ab34c9c6-792e-4f8e-b152-90cd8f524b9f"
            }
          ]
        },
        {
          "id": "781ce595-7929-4d0d-ba65-1d38fbed9864",
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
              "id": "ece0208a-6306-4d0a-8ce7-135289164632"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "5d34f97a-be7f-4792-931e-879bfbe977da",
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
              "id": "28296a00-384e-4caf-b03d-2b89d401639e"
            }
          ]
        }
      ]
    }
  ]
}