---
swagger: "2.0"
x-collection-name: 1Forge
x-complete: 0
info:
  title: 1Forge Get Currency Symbols API
  description: Get a list of currency symbols to use when making calls to the other
    APIs.
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
x-streamrank:
  polling_total_time_average: "0.58"
  polling_size_download_average: "312.37"
  streaming_total_time_average: "0.4"
  streaming_size_download_average: "161.9"
  change_yes: "2"
  change_no: "187"
  time_percentage: "31"
  size_percentage: "48"
  change_percentage: "1"
  last_run: "2018-02-19"
  days_run: "0"
  minute_run: "0"
---