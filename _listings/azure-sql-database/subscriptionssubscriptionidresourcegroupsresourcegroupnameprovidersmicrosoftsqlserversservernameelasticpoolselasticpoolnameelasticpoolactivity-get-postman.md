{
  "info": {
    "name": "Azure SQL Database API Elastic Pools List Activity",
    "_postman_id": "e46e9789-3fb6-46fe-9835-58e175648599",
    "description": "Returns elastic pool activities.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "elastic pools activity",
      "item": [
        {
          "id": "3b3ad03b-e8cd-499e-8b2d-13d29c76c052",
          "name": "ElasticPools_ListActivity",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/elasticPools/:elasticPoolName/elasticPoolActivity"
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
                  "id": "elasticPoolName",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "subscriptionId",
                  "value": "subscriptionId",
                  "type": "string"
                },
                {
                  "id": "resourceGroupName",
                  "value": "resourceGroupName",
                  "type": "string"
                },
                {
                  "id": "serverName",
                  "value": "serverName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns elastic pool activities"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "eb28355e-31c7-45fb-beb0-80d42b65118e"
            }
          ]
        }
      ]
    }
  ]
}