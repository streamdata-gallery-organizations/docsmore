{
  "info": {
    "name": "Docsmore Get All Document Flows",
    "_postman_id": "4854f5f5-3460-4949-a04b-132650abee93",
    "description": "Get all document flows.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Document",
      "item": [
        {
          "id": "761d3a9c-f62f-42ed-8be3-acb1163acd29",
          "name": "ApiDocflowGetdocflowsGet",
          "request": {
            "url": "http://api.docsmore.com/api/docflow/getdocflows",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get all document flows."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "daed4252-9685-4e22-8488-2ff000a2ffcf"
            }
          ]
        }
      ]
    }
  ]
}