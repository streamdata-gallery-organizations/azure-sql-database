---
swagger: "2.0"
x-collection-name: Azure SQL Database
x-complete: 0
info:
  title: Azure SQL Database API Operations List
  description: Lists all of the available SQL Rest API operations.
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenamerestorepoints-get
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
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftsqllocationslocationidcapabilities-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenamesecurityalertpoliciesdefault-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenamesecurityalertpoliciesdefault-put
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamefirewallrulesfirewallrulename-put
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
    delete:
      summary: Firewall Rules Delete
      description: Deletes a firewall rule.
      operationId: FirewallRules_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamefirewallrulesfirewallrulename-delete
      parameters:
      - in: path
        name: firewallRuleName
        description: The name of the firewall rule
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Firewall Rules
    get:
      summary: Firewall Rules Get
      description: Gets a firewall rule.
      operationId: FirewallRules_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamefirewallrulesfirewallrulename-get
      parameters:
      - in: path
        name: firewallRuleName
        description: The name of the firewall rule
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Firewall Rules
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/firewallRules:
    get:
      summary: Firewall Rules List By Server
      description: Returns a list of firewall rules.
      operationId: FirewallRules_ListByServer
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamefirewallrules-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Firewall Rules Server
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/import:
    post:
      summary: Databases Import
      description: Imports a bacpac into a new database.
      operationId: Databases_Import
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernameimport-post
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The required parameters for importing a Bacpac into a database
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Databases Import
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/extensions/import
  : put:
      summary: Databases Create Import Operation
      description: Creates an import operation that imports a bacpac into an existing
        database. The existing database must be empty.
      operationId: Databases_CreateImportOperation
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenameextensionsimport-put
      parameters:
      - in: path
        name: databaseName
        description: The name of the database to import into
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The required parameters for importing a Bacpac into a database
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Databases Import Operation
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/export
  : post:
      summary: Databases Export
      description: Exports a database to a bacpac.
      operationId: Databases_Export
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenameexport-post
      parameters:
      - in: path
        name: databaseName
        description: The name of the database to be exported
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The required parameters for exporting a database
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Databases Export
  /providers/Microsoft.Sql/operations:
    get:
      summary: Operations List
      description: Lists all of the available SQL Rest API operations.
      operationId: Operations_List
      x-api-path-slug: providersmicrosoftsqloperations-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Operations
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