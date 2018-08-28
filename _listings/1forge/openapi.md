---
swagger: "2.0"
x-collection-name: 1Forge
x-complete: 1
info:
  title: 1Forge
  description: 1forge-provides-realtime-quote-data-bid--ask-for-240-pairs--to-see-a-full-list-of-supported-currency-pairs-please-see-the-full-currency-pair-list--at-this-time-we-do-not-offer-historical-data-however-clients-are-more-than-welcome-to-archive-our-quotes-locally-for-internal-use-
  version: 1.0.0
host: forex.1forge.com
basePath: 1.0.3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /symbols:
    get:
      summary: Get Currency Symbols API
      description: Get a list of currency symbols to use when making calls to the
        other APIs.
      operationId: getSymbols
      x-api-path-slug: symbols-get
      parameters:
      - in: query
        name: api_key
        description: The api key
        type: string
        format: string
      - in: query
        name: format
        description: The format to return
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Symbols
---