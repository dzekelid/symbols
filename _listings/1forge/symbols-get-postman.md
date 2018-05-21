{
  "info": {
    "name": "1Forge Get Currency Symbols API",
    "_postman_id": "26362a40-a20e-464b-8aae-848ce2f0d623",
    "description": "Get a list of currency symbols to use when making calls to the other APIs.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Quotes",
      "item": [
        {
          "id": "8488e02d-3c15-42d8-afc0-b1d8a7b48656",
          "name": "getQuotes",
          "request": {
            "url": "http://forex.1forge.com/1.0.3/quotes?api_key=api_key&format=format&pairs=pairs",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get quotes for specific currency pair(s)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3305e32d-c712-4817-8a40-e48cefcb0fc4"
            }
          ]
        }
      ]
    },
    {
      "name": "Symbols",
      "item": [
        {
          "id": "e9c84549-0f3a-4488-ac01-234b9e937db2",
          "name": "getSymbols",
          "request": {
            "url": "http://forex.1forge.com/1.0.3/symbols?api_key=api_key&format=format",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get a list of currency symbols to use when making calls to the other APIs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd8b9683-e5d0-413c-b460-b5c089f56dcb"
            }
          ]
        }
      ]
    }
  ]
}