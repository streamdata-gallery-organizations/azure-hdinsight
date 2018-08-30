{
  "info": {
    "name": "HDInsightManagementClient",
    "_postman_id": "5ef11e4e-8a01-496d-99c3-ba7ec7a1d804",
    "description": "The HDInsight Management Client.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "applications",
      "item": [
        {
          "id": "702b5239-0e01-4a49-a47b-827cc4b77c68",
          "name": "Applications_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.HDInsight/clusters/:clusterName/applications/:applicationName"
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
                  "id": "applicationName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "clusterName",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all of the applications HDInsight cluster"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc7cee86-d5b3-4336-87e1-b614b4b86e78"
            }
          ]
        }
      ]
    }
  ]
}