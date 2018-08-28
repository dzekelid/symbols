swagger: "2.0"
x-collection-name: Xignite
x-complete: 1
info:
  title: Xignite VWAP
  description: provides-delayed-and-historical-volumeweightedaverage-price-vwap-information-
  version: 1.0.0
host: www.xignite.com
basePath: xVWAP.json/XigniteVWAP
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ListTradedSymbols:
    get:
      summary: List Traded Symbols
      description: Returns all symbols and names that are traded
      operationId: ListTradedSymbols
      x-api-path-slug: listtradedsymbols-get
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
  /ListSymbols:
    get:
      summary: List Symbols
      description: List available logos on market.
      operationId: postListsymbols
      x-api-path-slug: listsymbols-get
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
      - Symbols
  /GetFutureSymbol:
    get:
      summary: Get Future Symbol
      description: Returns the symbol for a future based on its month and year.
      operationId: postGetfuturesymbol
      x-api-path-slug: getfuturesymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Future
      - Symbol
  /GetReverseFutureSymbol:
    get:
      summary: Get Reverse Future Symbol
      description: Returns the symbol for a future based on its month and year.
      operationId: postGetreversefuturesymbol
      x-api-path-slug: getreversefuturesymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Reverse
      - Future
      - Symbol
  /GetIndexSymbolMappingsByOldSymbols:
    get:
      summary: Get Index Symbol Mappings By Old Symbols
      description: Get index symbol mappings by old symbols.
      operationId: GetIndexSymbolMappingsByOldSymbols
      x-api-path-slug: getindexsymbolmappingsbyoldsymbols-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Index
      - Symbol
      - Mappings
      - Old
      - Symbols
  /GetIndexSymbolMappingByOldSymbol:
    get:
      summary: Get Index Symbol Mapping By Old Symbol
      description: Get index symbol mapping by old symbol.
      operationId: GetIndexSymbolMappingByOldSymbol
      x-api-path-slug: getindexsymbolmappingbyoldsymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Index
      - Symbol
      - Mapping
      - Old
      - Symbol
  /ListSymbolChanges:
    get:
      summary: List Symbol Changes
      description: This operation returns symbols changed in this exchange.
      operationId: ListSymbolChanges
      x-api-path-slug: listsymbolchanges-get
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
      - Symbol
      - Changes
  /GetOptionBySymbol:
    get:
      summary: Get Option By Symbol
      description: Get details on an option.
      operationId: GetOptionBySymbol
      x-api-path-slug: getoptionbysymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Option
      - Symbol
  /GetEquityOptionBySymbols:
    get:
      summary: Get Equity Option By Symbols
      description: Returns an array of specific equity options.
      operationId: GetEquityOptionBySymbols
      x-api-path-slug: getequityoptionbysymbols-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Equity
      - Option
      - Symbols
  /GetExtendedEquityOptionBySymbols:
    get:
      summary: Get Extended Equity Option By Symbols
      description: Returns an array of specific equity extended options.
      operationId: GetExtendedEquityOptionBySymbols
      x-api-path-slug: getextendedequityoptionbysymbols-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Extended
      - Equity
      - Option
      - Symbols
  /GetEquityOptionSymbol:
    get:
      summary: Get Equity Option Symbol
      description: Returns the symbol for an equity option based on month, year and
        strike price.
      operationId: GetEquityOptionSymbol
      x-api-path-slug: getequityoptionsymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Equity
      - Option
      - Symbol
  /GetEquityOptionBySymbol:
    get:
      summary: Get Equity Option By Symbol
      description: Returns a specific equity option.
      operationId: GetEquityOptionBySymbol
      x-api-path-slug: getequityoptionbysymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Equity
      - Option
      - Symbol
  /GetExtendedEquityOptionBySymbol:
    get:
      summary: Get Extended Equity Option By Symbol
      description: Returns a specific equity extended option.
      operationId: GetExtendedEquityOptionBySymbol
      x-api-path-slug: getextendedequityoptionbysymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Extended
      - Equity
      - Option
      - Symbol
  /GetSymbols:
    get:
      summary: Get Symbols
      description: Returns a list of symbols available in the historical database.
      operationId: postGetsymbols
      x-api-path-slug: getsymbols-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Symbols
  /SearchIPOBySymbol:
    get:
      summary: Search IPO By Symbol
      description: Post searchipobysymbol
      operationId: SearchIPOBySymbol
      x-api-path-slug: searchipobysymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Search
      - IPO
      - Symbol
  /ListFundsBySymbol:
    get:
      summary: List Funds By Symbol
      description: This operation returns a list of funds descreptive information.
      operationId: ListFundsBySymbol
      x-api-path-slug: listfundsbysymbol-get
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
      - Funds
      - Symbol
  /GetRateSymbol:
    get:
      summary: Get Rate Symbol
      description: Returns the symbol for a rate.
      operationId: postGetratesymbol
      x-api-path-slug: getratesymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - Symbol
  /GetRateFromSymbol:
    get:
      summary: Get Rate From Symbol
      description: Returns the symbol for a rate.
      operationId: postGetratefromsymbol
      x-api-path-slug: getratefromsymbol-get
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Market Data
      - Rate
      - From
      - Symbol