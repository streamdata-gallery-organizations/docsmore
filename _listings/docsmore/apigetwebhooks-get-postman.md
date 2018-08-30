{
  "info": {
    "name": "Docsmore List all Webhooks",
    "_postman_id": "6e0628cd-9bc9-4604-9a49-160e72cd5682",
    "description": "List Webhooks that are both active and inactive. Inactive webhooks with webhook type of 'static' will be automatically removed during the nightly job process.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "4c48dab0-21b8-4f34-8cc1-287e69ca2597",
          "name": "ApiGetwebhooksGet",
          "request": {
            "url": "http://api.docsmore.com/api/getwebhooks",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List Webhooks that are both active and inactive. Inactive webhooks with webhook type of 'static' will be automatically removed during the nightly job process."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ec4ee5b-cc42-42e2-bc77-6babc46a02d3"
            }
          ]
        }
      ]
    }
  ]
}