---
name: Plentymarkets
x-slug: plentymarkets
description: plentymarkets is an all-in-one e-commerce ERP solution, which combines
  a comprehensive stock management system with a versatile shop system and effortless
  multichannel sales. Thanks to comprehensive functions and interfaces that include
  all steps of the e-commerce value chain, you can use the cloud based software to
  completely automate all of your e-business processes as well as your companys own
  individual processes.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
x-kinRank: "7"
x-alexaRank: ""
tags: Stocks
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/apis.md
specificationVersion: "0.14"
apis:
- name: plentymarkets REST-API - List stock of a variation per warehouse
  x-api-slug: restitemsidvariationsvariationidstock-get
  description: Lists stock of a variation per warehouse. The ID of the item and the
    ID of the variation must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstock-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstock-get-openapi.md
- name: plentymarkets REST-API - Book incoming stock
  x-api-slug: restitemsidvariationsvariationidstockbookincomingitems-put
  description: Books incoming stock for a variation. The incoming stock will be added
    to the existing stock. The ID of the item and the ID of the variation must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockbookincomingitems-put-openapi.md
- name: plentymarkets REST-API - Correct stock
  x-api-slug: restitemsidvariationsvariationidstockcorrection-put
  description: Corrects stock. The item ID and the variation ID must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockcorrection-put-openapi.md
- name: plentymarkets REST-API - List stock movements
  x-api-slug: restitemsidvariationsvariationidstockmovements-get
  description: |-
    Lists stock movements for a variation. The ID of the item and the ID of the variation must be specified. To get movements older than 3 months, set the 'year' parameter.
    NOTE: You can either get archive entries or non-archive entries. You can not get entries for the current year that are younger and older than 3 months with one request. You need separate requests to get entries older and younger than 3 months. To get all entries younger than 3 month you do not need to specify a year or any createdAt parameter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockmovements-get-openapi.md
- name: plentymarkets REST-API - Redistribute stock
  x-api-slug: restitemsidvariationsvariationidstockredistribute-put
  description: Redistributes the stock of one storage location among one or more storage
    locations. The item ID and the variation ID need to be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockredistribute-put-openapi.md
- name: plentymarkets REST-API - List stock of a variation per storage locations
  x-api-slug: restitemsidvariationsvariationidstockstoragelocations-get
  description: Lists stock of a variation per storage location. The ID of the item
    and the ID of the variation must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockstoragelocations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockstoragelocations-get-openapi.md
- name: plentymarkets REST-API - List listing stock dependence types
  x-api-slug: restlistingsstock-dependence-types-get
  description: Lists listing stock dependence types.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restlistingsstock-dependence-types-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restlistingsstock-dependence-types-get-openapi.md
- name: plentymarkets REST-API - Get a listing stock dependence type
  x-api-slug: restlistingsstock-dependence-typesid-get
  description: Gets a listing stock dependence type by given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restlistingsstock-dependence-typesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restlistingsstock-dependence-typesid-get-openapi.md
- name: plentymarkets REST-API - Revert outgoing stock
  x-api-slug: restordersorderidoutgoing-stocks-delete
  description: Reverts the booking of order items of an order. The ID of the order
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restordersorderidoutgoing-stocks-delete-openapi.md
- name: plentymarkets REST-API - List stock
  x-api-slug: reststockmanagementstock-get
  description: Lists stock of all warehouses.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementstock-get-openapi.md
- name: plentymarkets REST-API - Redistribute stock
  x-api-slug: reststockmanagementstockredistribute-put
  description: Redistributes stock of one storage location among one or more storage
    locations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementstockredistribute-put-openapi.md
- name: plentymarkets REST-API - List stock by warehouse type
  x-api-slug: reststockmanagementstocktypestype-get
  description: Lists stock for all warehouses of the same warehouse type. The name
    of the type must be specified. Currently the only type available is 'sales'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementstocktypestype-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementstocktypestype-get-openapi.md
- name: plentymarkets REST-API - List stock by warehouse
  x-api-slug: reststockmanagementwarehouseswarehouseidstock-get
  description: Lists stock for a warehouse. The ID of the warehouse must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementwarehouseswarehouseidstock-get-openapi.md
- name: plentymarkets REST-API - Book incoming stock
  x-api-slug: reststockmanagementwarehouseswarehouseidstockbookincomingitems-put
  description: Books incoming stock for multiple variations. The incoming stock will
    be added to the existing stock. The ID of the warehouse must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementwarehouseswarehouseidstockbookincomingitems-put-openapi.md
- name: plentymarkets REST-API - Correct stock
  x-api-slug: reststockmanagementwarehouseswarehouseidstockcorrection-put
  description: Corrects stock. The ID of the warehouse must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementwarehouseswarehouseidstockcorrection-put-openapi.md
- name: plentymarkets REST-API - List stock movements
  x-api-slug: reststockmanagementwarehouseswarehouseidstockmovements-get
  description: |-
    Lists stock movements for a warehouse. The ID of the warehouse must be specified. To get movements older than 3 months, set the 'year' parameter.
    NOTE: You can either get archive entries or non-archive entries. You can not get entries for the current year that are younger and older than 3 months with one request. You need separate requests to get entries older and younger than 3 months. To get all entries younger than 3 month you do not need to specify a year or any createdAt parameter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementwarehouseswarehouseidstockmovements-get-openapi.md
- name: plentymarkets REST-API - List stock of a warehouse per storage location
  x-api-slug: reststockmanagementwarehouseswarehouseidstockstoragelocations-get
  description: Lists stock of a warehouse for each variation and storage location.
    The stock will only be listed if the stock is positive. Negative stock will not
    be listed. The ID of the warehouse must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementwarehouseswarehouseidstockstoragelocations-get-openapi.md
- name: plentymarkets REST-API - List stock of a variation per warehouse
  x-api-slug: restitemsidvariationsvariationidstock-get
  description: Lists stock of a variation per warehouse. The ID of the item and the
    ID of the variation must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstock-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstock-get-openapi.md
- name: plentymarkets REST-API - Book incoming stock
  x-api-slug: restitemsidvariationsvariationidstockbookincomingitems-put
  description: Books incoming stock for a variation. The incoming stock will be added
    to the existing stock. The ID of the item and the ID of the variation must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockbookincomingitems-put-openapi.md
- name: plentymarkets REST-API - Correct stock
  x-api-slug: restitemsidvariationsvariationidstockcorrection-put
  description: Corrects stock. The item ID and the variation ID must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockcorrection-put-openapi.md
- name: plentymarkets REST-API - List stock movements
  x-api-slug: restitemsidvariationsvariationidstockmovements-get
  description: |-
    Lists stock movements for a variation. The ID of the item and the ID of the variation must be specified. To get movements older than 3 months, set the 'year' parameter.
    NOTE: You can either get archive entries or non-archive entries. You can not get entries for the current year that are younger and older than 3 months with one request. You need separate requests to get entries older and younger than 3 months. To get all entries younger than 3 month you do not need to specify a year or any createdAt parameter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockmovements-get-openapi.md
- name: plentymarkets REST-API - Redistribute stock
  x-api-slug: restitemsidvariationsvariationidstockredistribute-put
  description: Redistributes the stock of one storage location among one or more storage
    locations. The item ID and the variation ID need to be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockredistribute-put-openapi.md
- name: plentymarkets REST-API - List stock of a variation per storage locations
  x-api-slug: restitemsidvariationsvariationidstockstoragelocations-get
  description: Lists stock of a variation per storage location. The ID of the item
    and the ID of the variation must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockstoragelocations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockstoragelocations-get-openapi.md
- name: plentymarkets REST-API - List listing stock dependence types
  x-api-slug: restlistingsstock-dependence-types-get
  description: Lists listing stock dependence types.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restlistingsstock-dependence-types-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restlistingsstock-dependence-types-get-openapi.md
- name: plentymarkets REST-API - Get a listing stock dependence type
  x-api-slug: restlistingsstock-dependence-typesid-get
  description: Gets a listing stock dependence type by given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restlistingsstock-dependence-typesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restlistingsstock-dependence-typesid-get-openapi.md
- name: plentymarkets REST-API - Revert outgoing stock
  x-api-slug: restordersorderidoutgoing-stocks-delete
  description: Reverts the booking of order items of an order. The ID of the order
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restordersorderidoutgoing-stocks-delete-openapi.md
- name: plentymarkets REST-API - List stock
  x-api-slug: reststockmanagementstock-get
  description: Lists stock of all warehouses.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementstock-get-openapi.md
- name: plentymarkets REST-API - Redistribute stock
  x-api-slug: reststockmanagementstockredistribute-put
  description: Redistributes stock of one storage location among one or more storage
    locations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementstockredistribute-put-openapi.md
- name: plentymarkets REST-API - List stock by warehouse type
  x-api-slug: reststockmanagementstocktypestype-get
  description: Lists stock for all warehouses of the same warehouse type. The name
    of the type must be specified. Currently the only type available is 'sales'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementstocktypestype-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementstocktypestype-get-openapi.md
- name: plentymarkets REST-API - List stock by warehouse
  x-api-slug: reststockmanagementwarehouseswarehouseidstock-get
  description: Lists stock for a warehouse. The ID of the warehouse must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementwarehouseswarehouseidstock-get-openapi.md
- name: plentymarkets REST-API - Book incoming stock
  x-api-slug: reststockmanagementwarehouseswarehouseidstockbookincomingitems-put
  description: Books incoming stock for multiple variations. The incoming stock will
    be added to the existing stock. The ID of the warehouse must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementwarehouseswarehouseidstockbookincomingitems-put-openapi.md
- name: plentymarkets REST-API - Correct stock
  x-api-slug: reststockmanagementwarehouseswarehouseidstockcorrection-put
  description: Corrects stock. The ID of the warehouse must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementwarehouseswarehouseidstockcorrection-put-openapi.md
- name: plentymarkets REST-API - List stock movements
  x-api-slug: reststockmanagementwarehouseswarehouseidstockmovements-get
  description: |-
    Lists stock movements for a warehouse. The ID of the warehouse must be specified. To get movements older than 3 months, set the 'year' parameter.
    NOTE: You can either get archive entries or non-archive entries. You can not get entries for the current year that are younger and older than 3 months with one request. You need separate requests to get entries older and younger than 3 months. To get all entries younger than 3 month you do not need to specify a year or any createdAt parameter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementwarehouseswarehouseidstockmovements-get-openapi.md
- name: plentymarkets REST-API - List stock of a warehouse per storage location
  x-api-slug: reststockmanagementwarehouseswarehouseidstockstoragelocations-get
  description: Lists stock of a warehouse for each variation and storage location.
    The stock will only be listed if the stock is positive. Negative stock will not
    be listed. The ID of the warehouse must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementwarehouseswarehouseidstockstoragelocations-get-openapi.md
- name: plentymarkets REST-API - List stock of a warehouse per storage location
  x-api-slug: reststockmanagementwarehouseswarehouseidstockstoragelocations-get
  description: Lists stock of a warehouse for each variation and storage location.
    The stock will only be listed if the stock is positive. Negative stock will not
    be listed. The ID of the warehouse must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementwarehouseswarehouseidstockstoragelocations-get-openapi.md
- name: plentymarkets REST-API - List stock movements
  x-api-slug: reststockmanagementwarehouseswarehouseidstockmovements-get
  description: |-
    Lists stock movements for a warehouse. The ID of the warehouse must be specified. To get movements older than 3 months, set the 'year' parameter.
    NOTE: You can either get archive entries or non-archive entries. You can not get entries for the current year that are younger and older than 3 months with one request. You need separate requests to get entries older and younger than 3 months. To get all entries younger than 3 month you do not need to specify a year or any createdAt parameter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementwarehouseswarehouseidstockmovements-get-openapi.md
- name: plentymarkets REST-API - Correct stock
  x-api-slug: reststockmanagementwarehouseswarehouseidstockcorrection-put
  description: Corrects stock. The ID of the warehouse must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementwarehouseswarehouseidstockcorrection-put-openapi.md
- name: plentymarkets REST-API - Book incoming stock
  x-api-slug: reststockmanagementwarehouseswarehouseidstockbookincomingitems-put
  description: Books incoming stock for multiple variations. The incoming stock will
    be added to the existing stock. The ID of the warehouse must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementwarehouseswarehouseidstockbookincomingitems-put-openapi.md
- name: plentymarkets REST-API - List stock by warehouse
  x-api-slug: reststockmanagementwarehouseswarehouseidstock-get
  description: Lists stock for a warehouse. The ID of the warehouse must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementwarehouseswarehouseidstock-get-openapi.md
- name: plentymarkets REST-API - List stock by warehouse type
  x-api-slug: reststockmanagementstocktypestype-get
  description: Lists stock for all warehouses of the same warehouse type. The name
    of the type must be specified. Currently the only type available is 'sales'.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementstocktypestype-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementstocktypestype-get-openapi.md
- name: plentymarkets REST-API - Redistribute stock
  x-api-slug: reststockmanagementstockredistribute-put
  description: Redistributes stock of one storage location among one or more storage
    locations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementstockredistribute-put-openapi.md
- name: plentymarkets REST-API - List stock
  x-api-slug: reststockmanagementstock-get
  description: Lists stock of all warehouses.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/reststockmanagementstock-get-openapi.md
- name: plentymarkets REST-API - Revert outgoing stock
  x-api-slug: restordersorderidoutgoing-stocks-delete
  description: Reverts the booking of order items of an order. The ID of the order
    must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restordersorderidoutgoing-stocks-delete-openapi.md
- name: plentymarkets REST-API - Get a listing stock dependence type
  x-api-slug: restlistingsstock-dependence-typesid-get
  description: Gets a listing stock dependence type by given ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restlistingsstock-dependence-typesid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restlistingsstock-dependence-typesid-get-openapi.md
- name: plentymarkets REST-API - List listing stock dependence types
  x-api-slug: restlistingsstock-dependence-types-get
  description: Lists listing stock dependence types.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restlistingsstock-dependence-types-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restlistingsstock-dependence-types-get-openapi.md
- name: plentymarkets REST-API - List stock of a variation per storage locations
  x-api-slug: restitemsidvariationsvariationidstockstoragelocations-get
  description: Lists stock of a variation per storage location. The ID of the item
    and the ID of the variation must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockstoragelocations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockstoragelocations-get-openapi.md
- name: plentymarkets REST-API - Redistribute stock
  x-api-slug: restitemsidvariationsvariationidstockredistribute-put
  description: Redistributes the stock of one storage location among one or more storage
    locations. The item ID and the variation ID need to be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockredistribute-put-openapi.md
- name: plentymarkets REST-API - List stock movements
  x-api-slug: restitemsidvariationsvariationidstockmovements-get
  description: |-
    Lists stock movements for a variation. The ID of the item and the ID of the variation must be specified. To get movements older than 3 months, set the 'year' parameter.
    NOTE: You can either get archive entries or non-archive entries. You can not get entries for the current year that are younger and older than 3 months with one request. You need separate requests to get entries older and younger than 3 months. To get all entries younger than 3 month you do not need to specify a year or any createdAt parameter.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockmovements-get-openapi.md
- name: plentymarkets REST-API - Correct stock
  x-api-slug: restitemsidvariationsvariationidstockcorrection-put
  description: Corrects stock. The item ID and the variation ID must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockcorrection-put-openapi.md
- name: plentymarkets REST-API - Book incoming stock
  x-api-slug: restitemsidvariationsvariationidstockbookincomingitems-put
  description: Books incoming stock for a variation. The incoming stock will be added
    to the existing stock. The ID of the item and the ID of the variation must be
    specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstockbookincomingitems-put-openapi.md
- name: plentymarkets REST-API - List stock of a variation per warehouse
  x-api-slug: restitemsidvariationsvariationidstock-get
  description: Lists stock of a variation per warehouse. The ID of the item and the
    ID of the variation must be specified.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/plentymarkets.png
  humanURL: http://www.plentymarkets.co.uk
  baseURL: https://example.com//
  tags: ERP, Service API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstock-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/stocks/master/_listings/plentymarkets/restitemsidvariationsvariationidstock-get-openapi.md
x-common:
- type: x-blog-rss
  url: https://www.plentymarkets.co.uk/?ActionCall=WebActionRSS&rrss_id=1
- type: x-github
  url: https://github.com/plentymarkets
- type: x-twitter
  url: https://twitter.com/plentymarketsuk
- type: x-website
  url: http://www.plentymarkets.co.uk
- type: x-api-gallery
  url: http://pivotal.tracker.api.gallery.streamdata.io
- type: x-api-stack
  url: http://plentymarkets.stack.network
- type: x-blog
  url: https://www.plentymarkets.co.uk/blog/
- type: x-pricing
  url: https://www.plentymarkets.co.uk/prices/
- type: x-website
  url: https://www.plentymarkets.co.uk
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---