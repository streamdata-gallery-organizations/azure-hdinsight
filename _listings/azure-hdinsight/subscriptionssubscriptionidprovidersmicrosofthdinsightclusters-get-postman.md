{
  "info": {
    "name": "Azure HDInsight API Clusters List",
    "_postman_id": "726d1bc0-b29f-4555-9d91-0b1ca4e957b1",
    "description": "Lists HDInsight clusters under the subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "clusters",
      "item": [
        {
          "id": "845b8826-a1f9-40fa-8ad7-cb3656c3d1a3",
          "name": "Clusters_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.HDInsight/clusters"
              ],
              "query": [
                {
                  "key": "No Name",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists HDInsight clusters under the subscription"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a331bf0a-c04c-4065-8252-9a9eea36eaae"
            }
          ]
        }
      ]
    }
  ]
}