{
  "info": {
    "name": "Azure SQL Database API Elastic Pools List By Server",
    "_postman_id": "a4e20748-5db1-46d7-bc51-ba08e032e9a8",
    "description": "Returns a list of elastic pools in a server.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "elastic pools server",
      "item": [
        {
          "id": "60a0210d-ac65-4e73-9273-e8a933bdbec2",
          "name": "ElasticPools_ListByServer",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/elasticPools"
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
            "description": "Returns a list of elastic pools in a server"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5b3b7004-d6be-4f01-a713-bb8ddf5db167"
            }
          ]
        }
      ]
    }
  ]
}