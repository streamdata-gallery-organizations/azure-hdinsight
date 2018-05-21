{
  "info": {
    "name": "Azure HDInsight API Clusters Get",
    "_postman_id": "81ab10af-ff47-4b20-9893-bd00697eb21f",
    "description": "Gets the specified cluster.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "clusters",
      "item": [
        {
          "id": "da22ed34-6113-4ac8-939b-83d2b9b731b7",
          "name": "Clusters_Get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.HDInsight/clusters/:clusterName"
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
            "description": "Gets the specified cluster"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2ccbe08-b722-453f-ba76-c65529ded55a"
            }
          ]
        }
      ]
    }
  ]
}