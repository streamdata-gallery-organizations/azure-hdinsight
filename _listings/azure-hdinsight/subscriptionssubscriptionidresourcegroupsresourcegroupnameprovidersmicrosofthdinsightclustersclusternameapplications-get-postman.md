{
  "info": {
    "name": "HDInsightManagementClient",
    "_postman_id": "ae40da4c-292b-4df8-9200-cf712189ba5c",
    "description": "The HDInsight Management Client.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "applications",
      "item": [
        {
          "id": "fba59af8-4389-4869-a8f2-d70c35e2c958",
          "name": "Applications_List",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.HDInsight/clusters/:clusterName/applications"
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
            "description": "Lists all of the applications HDInsight cluster"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "339bdbd1-c1d8-47bd-83f8-c951ca9ed706"
            }
          ]
        }
      ]
    }
  ]
}