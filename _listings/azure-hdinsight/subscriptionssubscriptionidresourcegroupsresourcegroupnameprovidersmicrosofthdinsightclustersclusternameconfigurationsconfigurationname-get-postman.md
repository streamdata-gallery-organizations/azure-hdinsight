{
  "info": {
    "name": "Azure HDInsight API Configurations Get",
    "_postman_id": "bde895f4-929a-4e37-bf1a-37472b643ebc",
    "description": "The configuration object for the specified cluster.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "configurations",
      "item": [
        {
          "id": "84e9d319-03a7-4c95-9ef7-79e3463bf967",
          "name": "Configurations_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.HDInsight/clusters/:clusterName/configurations/:configurationName"
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
                  "id": "clusterName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "configurationName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "The configuration object for the specified cluster"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e445f116-928f-46cf-8a17-fb61ceb9aa39"
            }
          ]
        }
      ]
    }
  ]
}