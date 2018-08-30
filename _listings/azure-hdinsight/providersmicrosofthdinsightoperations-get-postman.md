{
  "info": {
    "name": "Azure HDInsight API Operations List",
    "_postman_id": "d2b26fc8-ad8c-4e38-90bc-800e9ef2e7a3",
    "description": "Lists all of the available HDInsight REST API operations.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "operations",
      "item": [
        {
          "id": "e62eab89-57a8-4c77-a7b3-021cec4b56e8",
          "name": "Operations_List",
          "request": {
            "url": "http://management.azure.com/providers/Microsoft.HDInsight/operations?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all of the available HDInsight REST API operations"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61fbaab7-65ef-4b59-852a-6394ada0594f"
            }
          ]
        }
      ]
    }
  ]
}