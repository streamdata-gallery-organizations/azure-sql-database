{
  "info": {
    "name": "Azure SQL Database API Elastic Pools Delete",
    "_postman_id": "5976709e-1d19-4362-a5ed-cc46387dc379",
    "description": "Deletes the elastic pool.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "elastic pools",
      "item": [
        {
          "id": "3dadda3f-7db1-4adb-9866-2319c373a6df",
          "name": "ElasticPools_Delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/elasticPools/:elasticPoolName"
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the elastic pool"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4eff38fb-18dd-4e6b-8d45-f6e0e9f9308c"
            }
          ]
        }
      ]
    }
  ]
}