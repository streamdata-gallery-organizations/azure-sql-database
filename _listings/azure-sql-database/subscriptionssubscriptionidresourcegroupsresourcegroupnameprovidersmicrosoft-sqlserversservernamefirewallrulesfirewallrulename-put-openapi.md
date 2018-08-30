---
swagger: "2.0"
x-collection-name: Azure SQL Database
x-complete: 0
info:
  title: Azure SQL Database API Firewall Rules Create Or Update
  description: Creates or updates a firewall rule.
  version: 1.0.0
host: management.azure.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/restorePoints
  : get:
      summary: Databases List Restore Points
      description: Returns a list of database restore points.
      operationId: Databases_ListRestorePoints
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamerestorepoints-get
      parameters:
      - in: path
        name: databaseName
        description: The name of the database from which to retrieve available restore
          points
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Restore Points
  /subscriptions/{subscriptionId}/providers/Microsoft.Sql/locations/{locationId}/capabilities:
    get:
      summary: Capabilities List By Location
      description: Gets the capabilities available for the specified location.
      operationId: Capabilities_ListByLocation
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-sqllocationslocationidcapabilities-get
      parameters:
      - in: path
        name: locationId
        description: The location id whose capabilities are retrieved
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Capabilities Location
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/securityAlertPolicies/default
  : get:
      summary: Databases Get Threat Detection Policy
      description: Gets a database's threat detection policy.
      operationId: Databases_GetThreatDetectionPolicy
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamesecurityalertpoliciesdefault-get
      parameters:
      - in: path
        name: databaseName
        description: The name of the database for which database Threat Detection
          policy is defined
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Threat Detection Policy
    put:
      summary: Databases Create Or Update Threat Detection Policy
      description: Creates or updates a database's threat detection policy.
      operationId: Databases_CreateOrUpdateThreatDetectionPolicy
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamesecurityalertpoliciesdefault-put
      parameters:
      - in: path
        name: databaseName
        description: The name of the database for which database Threat Detection
          policy is defined
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The database Threat Detection policy
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Databases Threat Detection Policy
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/firewallRules/{firewallRuleName}
  : put:
      summary: Firewall Rules Create Or Update
      description: Creates or updates a firewall rule.
      operationId: FirewallRules_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamefirewallrulesfirewallrulename-put
      parameters:
      - in: path
        name: firewallRuleName
        description: The name of the firewall rule
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The required parameters for creating or updating a firewall rule
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Firewall Rules
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---