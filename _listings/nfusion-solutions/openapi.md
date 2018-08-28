swagger: "2.0"
x-collection-name: nFusion Solutions
x-complete: 1
info:
  title: nFusion Solutions Market Data API v1
  description: nfusion-solutions-provides-rest-and-streaming-apis-that-deliver-enterprisegrade-financial-data--data-sets-include-realtime-and-historical-pricing-for-spot-prices-of-precious-metals-such-as-gold-silver-platinum-and-palladium-exchange-rates-for-major-currency-pairs-exchange-rates-for-crypto-currencies-such-as-btc-eth-and-ltc--all-api-access-requires-authentication--in-order-to-be-issued-access-credentials-you-must-first-enter-into-a-service-agreement-with-nfusion-solutions-and-acquire-a-commercial-license--for-information-on-how-to-obtain-a-licence-contact-salesnfusionsolutions-com-
  contact:
    name: nFusion Solutions
    url: https://nfusionsolutions.com/contact
    email: support@nfusionsolutions.com
  version: 1.0.0
host: api.nfusionsolutions.biz
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v{version}/Metals/spot/supported:
    get:
      summary: Get list of symbols supported by the spot endpoints
      description: Get list of symbols supported by the spot endpoints.
      operationId: ApiV{versionMetalsSpotSupportedGet
      x-api-path-slug: apivversionmetalsspotsupported-get
      parameters:
      - in: query
        name: format
        description: to override content negotiation specify a value of json or xml
      - in: query
        name: token
        description: auth token
      - in: path
        name: version
        description: The requested API version
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Symbols
      - Supported
      - By
      - Spot
      - Endpoints
  /api/v{version}/Metals/benchmark/supported:
    get:
      summary: Get list of symbols supported by the benchmark endpoints
      description: Get list of symbols supported by the benchmark endpoints.
      operationId: ApiV{versionMetalsBenchmarkSupportedGet
      x-api-path-slug: apivversionmetalsbenchmarksupported-get
      parameters:
      - in: query
        name: format
        description: to override content negotiation specify a value of json or xml
      - in: query
        name: token
        description: auth token
      - in: path
        name: version
        description: The requested API version
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Symbols
      - Supported
      - By
      - Benchmark
      - Endpoints