{
  "info": {
    "name": "Azure SQL Database API Capabilities List By Location",
    "_postman_id": "ef4fa6fc-16b3-43f6-9f65-3d488e3e7002",
    "description": "Gets the capabilities available for the specified location.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Databases Restore Points",
      "item": [
        {
          "id": "20d493bd-1e3c-4c8f-aec4-55b55cc6e36f",
          "name": "Databases_ListRestorePoints",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/resourceGroups/:resourceGroupName/providers/Microsoft.Sql/servers/:serverName/databases/:databaseName/restorePoints"
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
                  "id": "databaseName",
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
            "description": "Returns a list of database restore points."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "229e75de-550a-4529-9a74-d7e6d9d051d9"
            }
          ]
        }
      ]
    },
    {
      "name": "Capabilities Location",
      "item": [
        {
          "id": "36412caf-c100-4332-a301-fef4ce56d718",
          "name": "Capabilities_ListByLocation",
          "request": {
            "url": {
              "protocol": "http",
              "host": "management.azure.com",
              "path": [
                "subscriptions/:subscriptionId/providers/Microsoft.Sql/locations/:locationId/capabilities"
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
                  "id": "locationId",
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
            "description": "Gets the capabilities available for the specified location."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "efcadb3f-c944-45ac-851d-83cecfb7cbea"
            }
          ]
        }
      ]
    }
  ]
}