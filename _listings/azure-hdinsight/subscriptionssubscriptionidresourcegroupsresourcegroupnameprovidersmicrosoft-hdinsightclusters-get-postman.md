{
  "info": {
    "name": "Azure HDInsight API Clusters List By Resource Group",
    "_postman_id": "18c616d5-f5a0-434c-9ff0-aa5abd6d9c5b",
    "description": "List the HDInsight clusters in a resource group.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "clusters resource group",
      "item": [
        {
          "id": "6ceca2d3-127d-49c0-897a-9952c30530a2",
          "name": "Clusters_ListByResourceGroup",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.HDInsight/clusters"
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
            "description": "List the HDInsight clusters in a resource group"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ee5a0175-3a45-4c37-a36b-8e47f486c484"
            }
          ]
        }
      ]
    }
  ]
}