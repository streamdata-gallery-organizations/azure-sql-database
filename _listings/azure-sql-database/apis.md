---
name: Azure SQL Database
x-slug: azure-sql-database
description: Make building and maintaining applications easier and more productive.
  With built-in intelligence that learns app patterns and adapts to maximize performance,
  reliability, and data protection, SQL Database is a cloud database built for developers.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
x-kinRank: "10"
x-alexaRank: ""
tags: Azure SQL Database
created: "2018-05-24"
modified: "2018-05-24"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/apis.md
specificationVersion: "0.14"
apis:
- name: Azure SQL Database API Databases List Restore Points
  x-api-slug: azure-sql-database-api
  description: Returns a list of database restore points.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/restorePoints
  tags: Databases Restore Points
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamerestorepoints-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamerestorepoints-get-openapi.md
- name: Azure SQL Database API Capabilities List By Location
  x-api-slug: azure-sql-database-api
  description: Gets the capabilities available for the specified location.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Sql/locations/{locationId}/capabilities
  tags: Capabilities Location
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidprovidersmicrosoft-sqllocationslocationidcapabilities-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidprovidersmicrosoft-sqllocationslocationidcapabilities-get-openapi.md
- name: Azure SQL Database API Databases Get Threat Detection Policy
  x-api-slug: azure-sql-database-api
  description: Gets a database's threat detection policy.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/securityAlertPolicies/default
  tags: Databases Threat Detection Policy
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamesecurityalertpoliciesdefault-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamesecurityalertpoliciesdefault-get-openapi.md
- name: Azure SQL Database API Databases Create Or Update Threat Detection Policy
  x-api-slug: azure-sql-database-api
  description: Creates or updates a database's threat detection policy.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/securityAlertPolicies/default
  tags: Databases Threat Detection Policy
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamesecurityalertpoliciesdefault-put-openapi.md
- name: Azure SQL Database API Firewall Rules Create Or Update
  x-api-slug: azure-sql-database-api
  description: Creates or updates a firewall rule.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/firewallRules/{firewallRuleName}
  tags: Firewall Rules
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamefirewallrulesfirewallrulename-put-openapi.md
- name: Azure SQL Database API Firewall Rules Delete
  x-api-slug: azure-sql-database-api
  description: Deletes a firewall rule.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/firewallRules/{firewallRuleName}
  tags: Firewall Rules
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamefirewallrulesfirewallrulename-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamefirewallrulesfirewallrulename-delete-openapi.md
- name: Azure SQL Database API Firewall Rules Get
  x-api-slug: azure-sql-database-api
  description: Gets a firewall rule.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/firewallRules/{firewallRuleName}
  tags: Firewall Rules
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamefirewallrulesfirewallrulename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamefirewallrulesfirewallrulename-get-openapi.md
- name: Azure SQL Database API Firewall Rules List By Server
  x-api-slug: azure-sql-database-api
  description: Returns a list of firewall rules.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/firewallRules
  tags: Firewall Rules Server
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamefirewallrules-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamefirewallrules-get-openapi.md
- name: Azure SQL Database API Databases Import
  x-api-slug: azure-sql-database-api
  description: Imports a bacpac into a new database.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/import
  tags: Databases Import
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameimport-post-openapi.md
- name: Azure SQL Database API Databases Create Import Operation
  x-api-slug: azure-sql-database-api
  description: Creates an import operation that imports a bacpac into an existing
    database. The existing database must be empty.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/extensions/import
  tags: Databases Import Operation
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenameextensionsimport-put-openapi.md
- name: Azure SQL Database API Databases Export
  x-api-slug: azure-sql-database-api
  description: Exports a database to a bacpac.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/export
  tags: Databases Export
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenameexport-post-openapi.md
- name: Azure SQL Database API Operations List
  x-api-slug: azure-sql-database-api
  description: Lists all of the available SQL Rest API operations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////providers/Microsoft.Sql/operations
  tags: Operations
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/providersmicrosoft-sqloperations-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/providersmicrosoft-sqloperations-get-openapi.md
- name: Azure SQL Database API Databases Delete Replication Link
  x-api-slug: azure-sql-database-api
  description: Deletes a database replication link. Cannot be done during failover.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/replicationLinks/{linkId}
  tags: Databases Replication Link
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamereplicationlinkslinkid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamereplicationlinkslinkid-delete-openapi.md
- name: Azure SQL Database API Databases Get Replication Link
  x-api-slug: azure-sql-database-api
  description: Gets a database replication link.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/replicationLinks/{linkId}
  tags: Databases Replication Link
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamereplicationlinkslinkid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamereplicationlinkslinkid-get-openapi.md
- name: Azure SQL Database API Databases Failover Replication Link
  x-api-slug: azure-sql-database-api
  description: Sets which replica database is primary by failing over from the current
    primary replica database.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/replicationLinks/{linkId}/failover
  tags: Databases Failover Replication Link
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamereplicationlinkslinkidfailover-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamereplicationlinkslinkidfailover-post-openapi.md
- name: Azure SQL Database API Databases Failover Replication Link Allow Data Loss
  x-api-slug: azure-sql-database-api
  description: Sets which replica database is primary by failing over from the current
    primary replica database. This operation might result in data loss.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/replicationLinks/{linkId}/forceFailoverAllowDataLoss
  tags: Databases Failover Replication Link Allow Data Loss
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamereplicationlinkslinkidforcefailoverallowdataloss-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamereplicationlinkslinkidforcefailoverallowdataloss-post-openapi.md
- name: Azure SQL Database API Databases List Replication Links
  x-api-slug: azure-sql-database-api
  description: Lists a database's replication links.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/replicationLinks
  tags: Databases Replication Links
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamereplicationlinks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamereplicationlinks-get-openapi.md
- name: Azure SQL Database API Servers List
  x-api-slug: azure-sql-database-api
  description: Returns a list of servers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/providers/Microsoft.Sql/servers
  tags: Servers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidprovidersmicrosoft-sqlservers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidprovidersmicrosoft-sqlservers-get-openapi.md
- name: Azure SQL Database API Servers Create Or Update
  x-api-slug: azure-sql-database-api
  description: Creates or updates a new server.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}
  tags: Servers
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservername-put-openapi.md
- name: Azure SQL Database API Servers Delete
  x-api-slug: azure-sql-database-api
  description: Deletes a SQL server.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}
  tags: Servers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservername-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservername-delete-openapi.md
- name: Azure SQL Database API Servers Get
  x-api-slug: azure-sql-database-api
  description: Gets a server.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}
  tags: Servers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservername-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservername-get-openapi.md
- name: Azure SQL Database API Servers List By Resource Group
  x-api-slug: azure-sql-database-api
  description: Returns a list of servers in a resource group.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers
  tags: Servers Resource Group
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlservers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlservers-get-openapi.md
- name: Azure SQL Database API Servers List Usages
  x-api-slug: azure-sql-database-api
  description: Returns server usages.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/usages
  tags: Servers Usages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameusages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameusages-get-openapi.md
- name: Azure SQL Database API Databases Pause
  x-api-slug: azure-sql-database-api
  description: Pauses a data warehouse.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/pause
  tags: Databases Pause
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamepause-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenamepause-post-openapi.md
- name: Azure SQL Database API Databases Resume
  x-api-slug: azure-sql-database-api
  description: Resumes a data warehouse.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/resume
  tags: Databases Resume
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenameresume-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenameresume-post-openapi.md
- name: Azure SQL Database API Databases Create Or Update
  x-api-slug: azure-sql-database-api
  description: Creates a new database or updates an existing database. Location is
    a required property in the request body, and it must be the same as the location
    of the SQL server.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}
  tags: Databases
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasename-put-openapi.md
- name: Azure SQL Database API Databases Delete
  x-api-slug: azure-sql-database-api
  description: Deletes a database.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}
  tags: Databases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasename-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasename-delete-openapi.md
- name: Azure SQL Database API Databases Get
  x-api-slug: azure-sql-database-api
  description: Gets a database.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}
  tags: Databases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasename-get-openapi.md
- name: Azure SQL Database API Databases List By Server
  x-api-slug: azure-sql-database-api
  description: Returns a list of databases in a server.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases
  tags: Databases Server
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabases-get-openapi.md
- name: Azure SQL Database API Databases List Usages
  x-api-slug: azure-sql-database-api
  description: Returns database usages.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/usages
  tags: Databases Usages
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenameusages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenameusages-get-openapi.md
- name: Azure SQL Database API Elastic Pools Create Or Update
  x-api-slug: azure-sql-database-api
  description: Creates a new elastic pool or updates an existing elastic pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/elasticPools/{elasticPoolName}
  tags: Elastic Pools
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolname-put-openapi.md
- name: Azure SQL Database API Elastic Pools Delete
  x-api-slug: azure-sql-database-api
  description: Deletes the elastic pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/elasticPools/{elasticPoolName}
  tags: Elastic Pools
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolname-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolname-delete-openapi.md
- name: Azure SQL Database API Elastic Pools Get
  x-api-slug: azure-sql-database-api
  description: Gets an elastic pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/elasticPools/{elasticPoolName}
  tags: Elastic Pools
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolname-get-openapi.md
- name: Azure SQL Database API Elastic Pools List By Server
  x-api-slug: azure-sql-database-api
  description: Returns a list of elastic pools in a server.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/elasticPools
  tags: Elastic Pools Server
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpools-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpools-get-openapi.md
- name: Azure SQL Database API Elastic Pools List Activity
  x-api-slug: azure-sql-database-api
  description: Returns elastic pool activities.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/elasticPools/{elasticPoolName}/elasticPoolActivity
  tags: Elastic Pools Activity
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolnameelasticpoolactivity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolnameelasticpoolactivity-get-openapi.md
- name: Azure SQL Database API Elastic Pools List Database Activity
  x-api-slug: azure-sql-database-api
  description: Returns activity on databases inside of an elastic pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/elasticPools/{elasticPoolName}/elasticPoolDatabaseActivity
  tags: Elastic Pools Database Activity
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolnameelasticpooldatabaseactivity-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolnameelasticpooldatabaseactivity-get-openapi.md
- name: Azure SQL Database API Elastic Pools Get Database
  x-api-slug: azure-sql-database-api
  description: Gets a database inside of an elastic pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/elasticPools/{elasticPoolName}/databases/{databaseName}
  tags: Elastic Pools Database
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolnamedatabasesdatabasename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolnamedatabasesdatabasename-get-openapi.md
- name: Azure SQL Database API Elastic Pools List Databases
  x-api-slug: azure-sql-database-api
  description: Returns a list of databases in an elastic pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/elasticPools/{elasticPoolName}/databases
  tags: Elastic Pools Databases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolnamedatabases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameelasticpoolselasticpoolnamedatabases-get-openapi.md
- name: Azure SQL Database API Recommended Elastic Pools Get
  x-api-slug: azure-sql-database-api
  description: Gets a recommented elastic pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/recommendedElasticPools/{recommendedElasticPoolName}
  tags: Recommended Elastic Pools
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamerecommendedelasticpoolsrecommendedelasticpoolname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamerecommendedelasticpoolsrecommendedelasticpoolname-get-openapi.md
- name: Azure SQL Database API Recommended Elastic Pools Get Databases
  x-api-slug: azure-sql-database-api
  description: Gets a database inside of a recommented elastic pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/recommendedElasticPools/{recommendedElasticPoolName}/databases/{databaseName}
  tags: Recommended Elastic Pools Databases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamerecommendedelasticpoolsrecommendedelasticpoolnamedatabasesdatabasename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamerecommendedelasticpoolsrecommendedelasticpoolnamedatabasesdatabasename-get-openapi.md
- name: Azure SQL Database API Recommended Elastic Pools List By Server
  x-api-slug: azure-sql-database-api
  description: Returns recommended elastic pools.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/recommendedElasticPools
  tags: Recommended Elastic Pools Server
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamerecommendedelasticpools-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamerecommendedelasticpools-get-openapi.md
- name: Azure SQL Database API Recommended Elastic Pools List Databases
  x-api-slug: azure-sql-database-api
  description: Returns a list of databases inside a recommented elastic pool.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/recommendedElasticPools/{recommendedElasticPoolName}/databases
  tags: Recommended Elastic Pools Databases
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamerecommendedelasticpoolsrecommendedelasticpoolnamedatabases-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamerecommendedelasticpoolsrecommendedelasticpoolnamedatabases-get-openapi.md
- name: Azure SQL Database API Recommended Elastic Pools List Metrics
  x-api-slug: azure-sql-database-api
  description: Returns a recommented elastic pool metrics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/recommendedElasticPools/{recommendedElasticPoolName}/metrics
  tags: Recommended Elastic Pools Metrics
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamerecommendedelasticpoolsrecommendedelasticpoolnamemetrics-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamerecommendedelasticpoolsrecommendedelasticpoolnamemetrics-get-openapi.md
- name: Azure SQL Database API Databases Get Service Tier Advisor
  x-api-slug: azure-sql-database-api
  description: Gets a service tier advisor.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/serviceTierAdvisors/{serviceTierAdvisorName}
  tags: Databases Service Tier Advisor
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenameservicetieradvisorsservicetieradvisorname-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenameservicetieradvisorsservicetieradvisorname-get-openapi.md
- name: Azure SQL Database API Databases List Service Tier Advisors
  x-api-slug: azure-sql-database-api
  description: Returns service tier advisors for specified database.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/serviceTierAdvisors
  tags: Databases Service Tier Advisors
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenameservicetieradvisors-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenameservicetieradvisors-get-openapi.md
- name: Azure SQL Database API Servers Get Service Objective
  x-api-slug: azure-sql-database-api
  description: Gets a database service objective.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/serviceObjectives/{serviceObjectiveName}
  tags: Servers Service Objective
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameserviceobjectivesserviceobjectivename-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameserviceobjectivesserviceobjectivename-get-openapi.md
- name: Azure SQL Database API Servers List Service Objectives
  x-api-slug: azure-sql-database-api
  description: Returns database service objectives.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/serviceObjectives
  tags: Servers Service Objectives
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameserviceobjectives-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernameserviceobjectives-get-openapi.md
- name: Azure SQL Database API Databases Create Or Update Transparent Data Encryption
    Configuration
  x-api-slug: azure-sql-database-api
  description: Creates or updates a database's transparent data encryption configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/transparentDataEncryption/current
  tags: Databases Transparent Data Encryption Configuration
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenametransparentdataencryptioncurrent-put-openapi.md
- name: Azure SQL Database API Databases Get Transparent Data Encryption Configuration
  x-api-slug: azure-sql-database-api
  description: Gets a database's transparent data encryption configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/transparentDataEncryption/current
  tags: Databases Transparent Data Encryption Configuration
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenametransparentdataencryptioncurrent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenametransparentdataencryptioncurrent-get-openapi.md
- name: Azure SQL Database API Databases List Transparent Data Encryption Activity
  x-api-slug: azure-sql-database-api
  description: Returns a database's transparent data encryption operation result.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com////subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.Sql/servers/{serverName}/databases/{databaseName}/transparentDataEncryption/current/operationResults
  tags: Databases Transparent Data Encryption Activity
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenametransparentdataencryptioncurrentoperationresults-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosoft-sqlserversservernamedatabasesdatabasenametransparentdataencryptioncurrentoperationresults-get-openapi.md
- name: Azure SQL Database API
  x-api-slug: azure-sql-database-api
  description: Make building and maintaining applications easier and more productive.
    With built-in intelligence that learns app patterns and adapts to maximize performance,
    reliability, and data protection, SQL Database is a cloud database built for developers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/azure-sql-01-stop-worrying.png
  humanURL: https://azure.microsoft.com/en-us/services/sql-database/
  baseURL: ://management.azure.com//
  tags: Azure SQL Database
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/azure-sql-database/master/_listings/azure-sql-database/openapi.md
x-common:
- type: x-documentation
  url: https://docs.microsoft.com/en-us/azure/sql-database/
- type: x-pricing
  url: https://azure.microsoft.com/en-us/pricing/details/sql-database/
- type: x-service-level-agreements
  url: https://azure.microsoft.com/en-us/support/legal/sla/sql-database/
- type: x-status
  url: https://azure.microsoft.com/en-us/status/
- type: x-website
  url: https://azure.microsoft.com/en-us/services/sql-database/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---