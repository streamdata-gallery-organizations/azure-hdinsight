---
swagger: "2.0"
x-collection-name: Azure HDInsight
x-complete: 1
info:
  title: HDInsightManagementClient
  description: the-hdinsight-management-client
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
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/applications
  : get:
      summary: Applications List
      description: Lists all of the applications HDInsight cluster.
      operationId: Applications_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternameapplications-get
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Applications
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/applications/{applicationName}
  : get:
      summary: Applications Get
      description: Lists properties of the application.
      operationId: Applications_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternameapplicationsapplicationname-get
      parameters:
      - in: path
        name: applicationName
        description: The constant value for the applicationName
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Applications
    put:
      summary: Applications Create
      description: The operation creates applications for the HDInsight cluster.
      operationId: Applications_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternameapplicationsapplicationname-put
      parameters:
      - in: path
        name: applicationName
        description: The constant value for the applicationName
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The application create request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Applications
    delete:
      summary: Applications Delete
      description: Lists all of the applications HDInsight cluster.
      operationId: Applications_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternameapplicationsapplicationname-delete
      parameters:
      - in: path
        name: applicationName
        description: The constant value for the applicationName
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Applications
  /subscriptions/{subscriptionId}/providers/Microsoft.HDInsight/locations/{location}/capabilities:
    get:
      summary: Location Get Capabilities
      description: Gets the capabilities for the specified location.
      operationId: Location_GetCapabilities
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosofthdinsightlocationslocationcapabilities-get
      parameters:
      - in: path
        name: location
        description: The location to get capabilities for
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Location Capabilities
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}:
    put:
      summary: Clusters Create
      description: Begins creating a new HDInsight cluster with the specified parameters.
      operationId: Clusters_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclustername-put
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The cluster create request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Clusters
    patch:
      summary: Clusters Update
      description: Patch HDInsight cluster with the specified parameters.
      operationId: Clusters_Update
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclustername-patch
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The cluster patch request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Clusters
    delete:
      summary: Clusters Delete
      description: Begins deleting the specified HDInsight cluster.
      operationId: Clusters_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclustername-delete
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Clusters
    get:
      summary: Clusters Get
      description: Gets the specified cluster.
      operationId: Clusters_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclustername-get
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Clusters
  /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters:
    get:
      summary: Clusters List By Resource Group
      description: List the HDInsight clusters in a resource group.
      operationId: Clusters_ListByResourceGroup
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclusters-get
      parameters:
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Clusters Resource Group
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/roles/{roleName}/resize
  : post:
      summary: Clusters Resize
      description: Begins a resize operation on the specified HDInsight cluster.
      operationId: Clusters_Resize
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternamerolesrolenameresize-post
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters for the resize operation
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: roleName
        description: The constant value for the roleName
      responses:
        200:
          description: OK
      tags:
      - Clusters Resize
  /subscriptions/{subscriptionId}/providers/Microsoft.HDInsight/clusters:
    get:
      summary: Clusters List
      description: Lists HDInsight clusters under the subscription.
      operationId: Clusters_List
      x-api-path-slug: subscriptionssubscriptionidprovidersmicrosofthdinsightclusters-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Clusters
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/changerdpsetting
  : post:
      summary: Clusters Change Rdp Settings
      description: Begins changing the RDP settings on the specified cluster.
      operationId: Clusters_ChangeRdpSettings
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternamechangerdpsetting-post
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The OS profile for RDP
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Clusters Change Rdptings
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/configurations/{configurationName}
  : post:
      summary: Configurations Update HTTPSettings
      description: Begins configuring the HTTP settings on the specified cluster.
      operationId: Configurations_UpdateHTTPSettings
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternameconfigurationsconfigurationname-post
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: path
        name: configurationName
        description: The constant for configuration type of gateway
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The name of the resource group
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Configurations Httpsettings
    get:
      summary: Configurations Get
      description: The configuration object for the specified cluster.
      operationId: Configurations_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternameconfigurationsconfigurationname-get
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: path
        name: configurationName
        description: The constant for configuration type of gateway
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Configurations
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/extensions/{extensionName}
  : put:
      summary: Extension Create
      description: Create HDInsight cluster extension.
      operationId: Extension_Create
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternameextensionsextensionname-put
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: path
        name: extensionName
        description: The name of the cluster extension
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The cluster extensions create request
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Extension
    get:
      summary: Extension Get
      description: Get extension properties for HDInsight cluster extension.
      operationId: Extension_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternameextensionsextensionname-get
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: path
        name: extensionName
        description: The name of the cluster extension
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Extension
    delete:
      summary: Extension Delete
      description: Delete extension for HDInsight cluster.
      operationId: Extension_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternameextensionsextensionname-delete
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: path
        name: extensionName
        description: The name of the cluster extension
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Extension
  /providers/Microsoft.HDInsight/operations:
    get:
      summary: Operations List
      description: Lists all of the available HDInsight REST API operations.
      operationId: Operations_List
      x-api-path-slug: providersmicrosofthdinsightoperations-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Operations
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/scriptActions/{scriptName}
  : delete:
      summary: Script Actions Delete
      description: Deletes a given persisted script action of the cluster.
      operationId: ScriptActions_Delete
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternamescriptactionsscriptname-delete
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: scriptName
        description: The name of the script
      responses:
        200:
          description: OK
      tags:
      - Script Actions
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/executeScriptActions
  : post:
      summary: Clusters Execute Script Actions
      description: Begins executing script actions on the specified HDInsight cluster.
      operationId: Clusters_ExecuteScriptActions
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternameexecutescriptactions-post
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: body
        name: parameters
        description: The parameters for executing script actions
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Clusters Execute Script Actions
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/scriptActions
  : get:
      summary: Script Actions List
      description: Lists all persisted script actions for the given cluster.
      operationId: ScriptActions_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternamescriptactions-get
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Script Actions
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/scriptExecutionHistory/{scriptExecutionId}
  : get:
      summary: Script Execution History Get
      description: Gets the script execution detail for the given script execution
        id.
      operationId: ScriptExecutionHistory_Get
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternamescriptexecutionhistoryscriptexecutionid-get
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: scriptExecutionId
        description: The script execution Id
      responses:
        200:
          description: OK
      tags:
      - Script Execution History
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/scriptExecutionHistory
  : get:
      summary: Script Execution History List
      description: Lists all scripts execution history for the given cluster.
      operationId: ScriptExecutionHistory_List
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternamescriptexecutionhistory-get
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      responses:
        200:
          description: OK
      tags:
      - Script Execution History
  ? /subscriptions/{subscriptionId}/resourceGroups/{resourceGroupName}/providers/Microsoft.HDInsight/clusters/{clusterName}/scriptExecutionHistory/{scriptExecutionId}/promote
  : post:
      summary: Script Execution History Promote
      description: Promote ad-hoc script execution to a persisted script.
      operationId: ScriptExecutionHistory_Promote
      x-api-path-slug: subscriptionssubscriptionidresourcegroupsresourcegroupnameprovidersmicrosofthdinsightclustersclusternamescriptexecutionhistoryscriptexecutionidpromote-post
      parameters:
      - in: path
        name: clusterName
        description: The name of the cluster
      - in: query
        name: No Name
      - in: path
        name: resourceGroupName
        description: The name of the resource group
      - in: path
        name: scriptExecutionId
        description: The script execution Id
      responses:
        200:
          description: OK
      tags:
      - Script Execution History Promote
---