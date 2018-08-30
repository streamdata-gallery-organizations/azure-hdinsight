{
  "info": {
    "name": "HDInsightManagementClient",
    "_postman_id": "1b18da43-b26a-4b2d-a92a-fc0efaa5e471",
    "description": "The HDInsight Management Client.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "applications",
      "item": [
        {
          "id": "34cde472-c48a-4061-865c-69e2c34963cc",
          "name": "Applications_Get",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists properties of the application"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "50021edd-056d-40fc-bd70-f91d0c692326"
            }
          ]
        }
      ]
    }
  ]
}