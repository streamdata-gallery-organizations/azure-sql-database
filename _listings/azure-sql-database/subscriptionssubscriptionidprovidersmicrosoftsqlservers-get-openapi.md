---
swagger: "2.0"
x-collection-name: Azure SQL Database
x-complete: 0
info:
  title: Azure SQL Database API Servers List
  description: Returns a list of servers.
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/replicationLinks/{linkId}
  : delete:
      summary: Databases Delete Replication Link
      description: Deletes a database replication link. Cannot be done during failover.
      operationId: Databases_DeleteReplicationLink
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenamereplicationlinkslinkid-delete
      parameters:
      - in: path
        name: databaseName
        description: The name of the database that has the replication link to be
          dropped
      - in: path
        name: linkId
        description: The ID of the replication link to be deleted
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Replication Link
    get:
      summary: Databases Get Replication Link
      description: Gets a database replication link.
      operationId: Databases_GetReplicationLink
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenamereplicationlinkslinkid-get
      parameters:
      - in: path
        name: databaseName
        description: The name of the database to get the link for
      - in: path
        name: linkId
        description: The replication link ID to be retrieved
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Replication Link
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/replicationLinks/{linkId}/failover
  : post:
      summary: Databases Failover Replication Link
      description: Sets which replica database is primary by failing over from the
        current primary replica database.
      operationId: Databases_FailoverReplicationLink
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenamereplicationlinkslinkidfailover-post
      parameters:
      - in: path
        name: databaseName
        description: The name of the database that has the replication link to be
          failed over
      - in: path
        name: linkId
        description: The ID of the replication link to be failed over
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Failover Replication Link
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/replicationLinks/{linkId}/forceFailoverAllowDataLoss
  : post:
      summary: Databases Failover Replication Link Allow Data Loss
      description: Sets which replica database is primary by failing over from the
        current primary replica database. This operation might result in data loss.
      operationId: Databases_FailoverReplicationLinkAllowDataLoss
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenamereplicationlinkslinkidforcefailoverallowdataloss-post
      parameters:
      - in: path
        name: databaseName
        description: The name of the database that has the replication link to be
          failed over
      - in: path
        name: linkId
        description: The ID of the replication link to be failed over
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Failover Replication Link Allow Data Loss
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/replicationLinks
  : get:
      summary: Databases List Replication Links
      description: Lists a database's replication links.
      operationId: Databases_ListReplicationLinks
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoftsqlserversservernamedatabasesdatabasenamereplicationlinks-get
      parameters:
      - in: path
        name: databaseName
        description: The name of the database to retrieve links for
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Replication Links
  /subscriptions/{subscriptionId}/providers/Microsoft.Sql/servers:
    get:
      summary: Servers List
      description: Returns a list of servers.
      operationId: Servers_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoftsqlservers-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Servers
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