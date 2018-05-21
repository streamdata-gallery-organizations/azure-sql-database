{
  "info": {
    "name": "Azure SQL Database API Operations List",
    "_postman_id": "586d55a5-0aed-4a4e-acae-12e5cbb102f3",
    "description": "Lists all of the available SQL Rest API operations.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "operations",
      "item": [
        {
          "id": "c706a487-12b7-4055-a45a-8d04f1e949cd",
          "name": "Operations_List",
          "request": {
            "url": "http://management.azure.com/providers/Microsoft.Sql/operations?No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Lists all of the available SQL Rest API operations"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1032f8e3-ff18-41fe-a050-d757e361289b"
            }
          ]
        }
      ]
    }
  ]
}