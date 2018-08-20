{
  "info": {
    "name": "nFusion API Get historical prices for requested currency pairs",
    "_postman_id": "a2001193-f093-4034-8fa5-e4d4b11d4859",
    "description": "Historical OHLC data for the specified period and interval size\r\n\r\nThe combination of the interval parameter and start and end dates can result in results\r\nbeing truncated to conform to result size limits. See comments on interval parameter for details on valid interval values.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Historical",
      "item": [
        {
          "id": "e4956be6-59b7-403c-9bc5-134427b6f543",
          "name": "ApiV{versionCurrenciesHistoryGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.nfusionsolutions.biz",
              "path": [
                "api/v:version/Currencies/history"
              ],
              "query": [
                {
                  "key": "end",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "format",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "interval",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pairs",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "start",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "token",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "version",
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
            "description": "Historical OHLC data for the specified period and interval size\r\n\r\nThe combination of the interval parameter and start and end dates can result in results\r\nbeing truncated to conform to result size limits. See comments on interval parameter for details on valid interval values."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d18113d1-07b7-4bd2-859b-5a64a0d4f226"
            }
          ]
        }
      ]
    }
  ]
}