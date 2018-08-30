---
swagger: "2.0"
x-collection-name: Azure SQL Database
x-complete: 0
info:
  title: Azure SQL Database API Elastic Pools List Databases
  description: Returns a list of databases in an elastic pool.
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
    delete:
      summary: Firewall Rules Delete
      description: Deletes a firewall rule.
      operationId: FirewallRules_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamefirewallrulesfirewallrulename-delete
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamefirewallrulesfirewallrulename-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamefirewallrules-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameimport-post
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenameextensionsimport-put
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenameexport-post
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
      x-api-path-slug: providersmicrosoft-sqloperations-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamereplicationlinkslinkid-delete
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamereplicationlinkslinkid-get
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamereplicationlinkslinkidfailover-post
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamereplicationlinkslinkidforcefailoverallowdataloss-post
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
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamereplicationlinks-get
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
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosoft-sqlservers-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Servers
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}:
    put:
      summary: Servers Create Or Update
      description: Creates or updates a new server.
      operationId: Servers_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservername-put
      parameters:
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The required parameters for creating or updating a server
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Servers
    delete:
      summary: Servers Delete
      description: Deletes a SQL server.
      operationId: Servers_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservername-delete
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Servers
    get:
      summary: Servers Get
      description: Gets a server.
      operationId: Servers_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservername-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Servers
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers:
    get:
      summary: Servers List By Resource Group
      description: Returns a list of servers in a resource group.
      operationId: Servers_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlservers-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Servers Resource Group
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/usages:
    get:
      summary: Servers List Usages
      description: Returns server usages.
      operationId: Servers_ListUsages
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameusages-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Servers Usages
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/pause
  : post:
      summary: Databases Pause
      description: Pauses a data warehouse.
      operationId: Databases_Pause
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamepause-post
      parameters:
      - in: path
        name: databaseName
        description: The name of the data warehouse to pause
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Pause
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/resume
  : post:
      summary: Databases Resume
      description: Resumes a data warehouse.
      operationId: Databases_Resume
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenameresume-post
      parameters:
      - in: path
        name: databaseName
        description: The name of the data warehouse to resume
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Resume
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}
  : put:
      summary: Databases Create Or Update
      description: Creates a new database or updates an existing database. Location
        is a required property in the request body, and it must be the same as the
        location of the SQL server.
      operationId: Databases_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasename-put
      parameters:
      - in: path
        name: databaseName
        description: The name of the database to be operated on (updated or created)
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The required parameters for creating or updating a database
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Databases
    delete:
      summary: Databases Delete
      description: Deletes a database.
      operationId: Databases_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasename-delete
      parameters:
      - in: path
        name: databaseName
        description: The name of the database to be deleted
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases
    get:
      summary: Databases Get
      description: Gets a database.
      operationId: Databases_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasename-get
      parameters:
      - in: path
        name: databaseName
        description: The name of the database to be retrieved
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases:
    get:
      summary: Databases List By Server
      description: Returns a list of databases in a server.
      operationId: Databases_ListByServer
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabases-get
      parameters:
      - in: query
        name: $filter
        description: An OData filter expression that describes a subset of databases
          to return
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Server
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/usages
  : get:
      summary: Databases List Usages
      description: Returns database usages.
      operationId: Databases_ListUsages
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenameusages-get
      parameters:
      - in: path
        name: databaseName
        description: The name of the database
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Databases Usages
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/elasticPools/{elasticPoolName}
  : put:
      summary: Elastic Pools Create Or Update
      description: Creates a new elastic pool or updates an existing elastic pool.
      operationId: ElasticPools_CreateOrUpdate
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolname-put
      parameters:
      - in: path
        name: elasticPoolName
        description: The name of the elastic pool to be operated on (updated or created)
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The required parameters for creating or updating an elastic pool
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Elastic Pools
    delete:
      summary: Elastic Pools Delete
      description: Deletes the elastic pool.
      operationId: ElasticPools_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolname-delete
      parameters:
      - in: path
        name: elasticPoolName
        description: The name of the elastic pool to be deleted
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Elastic Pools
    get:
      summary: Elastic Pools Get
      description: Gets an elastic pool.
      operationId: ElasticPools_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolname-get
      parameters:
      - in: path
        name: elasticPoolName
        description: The name of the elastic pool to be retrieved
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Elastic Pools
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/elasticPools:
    get:
      summary: Elastic Pools List By Server
      description: Returns a list of elastic pools in a server.
      operationId: ElasticPools_ListByServer
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpools-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Elastic Pools Server
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/elasticPools/{elasticPoolName}/elasticPoolActivity
  : get:
      summary: Elastic Pools List Activity
      description: Returns elastic pool activities.
      operationId: ElasticPools_ListActivity
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolnameelasticpoolactivity-get
      parameters:
      - in: path
        name: elasticPoolName
        description: The name of the elastic pool for which to get the current activity
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Elastic Pools Activity
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/elasticPools/{elasticPoolName}/elasticPoolDatabaseActivity
  : get:
      summary: Elastic Pools List Database Activity
      description: Returns activity on databases inside of an elastic pool.
      operationId: ElasticPools_ListDatabaseActivity
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolnameelasticpooldatabaseactivity-get
      parameters:
      - in: path
        name: elasticPoolName
        description: The name of the elastic pool
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Elastic Pools Database Activity
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/elasticPools/{elasticPoolName}/databases/{databaseName}
  : get:
      summary: Elastic Pools Get Database
      description: Gets a database inside of an elastic pool.
      operationId: ElasticPools_GetDatabase
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolnamedatabasesdatabasename-get
      parameters:
      - in: path
        name: databaseName
        description: The name of the database to be retrieved
      - in: path
        name: elasticPoolName
        description: The name of the elastic pool to be retrieved
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Elastic Pools Database
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/elasticPools/{elasticPoolName}/databases
  : get:
      summary: Elastic Pools List Databases
      description: Returns a list of databases in an elastic pool.
      operationId: ElasticPools_ListDatabases
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolnamedatabases-get
      parameters:
      - in: path
        name: elasticPoolName
        description: The name of the elastic pool to be retrieved
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Elastic Pools Databases
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