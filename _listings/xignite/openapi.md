---
swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite NASDAQ Last Sale
  description: provides-realtime-access-to-last-sale-nasdaq-amex-and-nyse-information
  version: 1.0.0
host: nasdaqlastsale.xignite.com
basePath: xNASDAQLastSale.json/XigniteNASDAQLastSale
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ListTradedSymbols:
    post:
      summary: List Traded Symbols
      description: Returns all symbols and names that are traded
      operationId: ListTradedSymbols
      x-api-path-slug: listtradedsymbols-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Traded
      - Symbols
---