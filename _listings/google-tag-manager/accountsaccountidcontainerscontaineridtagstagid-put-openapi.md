---
swagger: "2.0"
x-collection-name: Google Tag Manager
x-complete: 0
info:
  title: Google Tag Manager API Update GTM Tag
  description: Updates a GTM Tag.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /tagmanager/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts:
    get:
      summary: Get Accounts
      description: Lists all GTM Accounts that a user has access to.
      operationId: tagmanager.accounts.list
      x-api-path-slug: accounts-get
      responses:
        200:
          description: OK
      tags:
      - Account
  /accounts/{accountId}:
    get:
      summary: Get Account
      description: Gets a GTM Account.
      operationId: tagmanager.accounts.get
      x-api-path-slug: accountsaccountid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      responses:
        200:
          description: OK
      tags:
      - Account
    put:
      summary: Update Account
      description: Updates a GTM Account.
      operationId: tagmanager.accounts.update
      x-api-path-slug: accountsaccountid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the account in storage
      responses:
        200:
          description: OK
      tags:
      - Account
  /accounts/{accountId}/containers:
    get:
      summary: Get Conainers
      description: Lists all Containers that belongs to a GTM Account.
      operationId: tagmanager.accounts.containers.list
      x-api-path-slug: accountsaccountidcontainers-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      responses:
        200:
          description: OK
      tags:
      - Container
    post:
      summary: Create Container
      description: Creates a Container.
      operationId: tagmanager.accounts.containers.create
      x-api-path-slug: accountsaccountidcontainers-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Container
  /accounts/{accountId}/containers/{containerId}:
    delete:
      summary: Delete Container
      description: Deletes a Container.
      operationId: tagmanager.accounts.containers.delete
      x-api-path-slug: accountsaccountidcontainerscontainerid-delete
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - Container
    get:
      summary: Get Container
      description: Gets a Container.
      operationId: tagmanager.accounts.containers.get
      x-api-path-slug: accountsaccountidcontainerscontainerid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - Container
    put:
      summary: Update Container
      description: Updates a Container.
      operationId: tagmanager.accounts.containers.update
      x-api-path-slug: accountsaccountidcontainerscontainerid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the container in storage
      responses:
        200:
          description: OK
      tags:
      - Container
  /accounts/{accountId}/containers/{containerId}/environments:
    get:
      summary: Get GTM Environments
      description: Lists all GTM Environments of a GTM Container.
      operationId: tagmanager.accounts.containers.environments.list
      x-api-path-slug: accountsaccountidcontainerscontaineridenvironments-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Environment
    post:
      summary: Create GTM Environment
      description: Creates a GTM Environment.
      operationId: tagmanager.accounts.containers.environments.create
      x-api-path-slug: accountsaccountidcontainerscontaineridenvironments-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Environment
  /accounts/{accountId}/containers/{containerId}/environments/{environmentId}:
    delete:
      summary: Delete GTM Environment
      description: Deletes a GTM Environment.
      operationId: tagmanager.accounts.containers.environments.delete
      x-api-path-slug: accountsaccountidcontainerscontaineridenvironmentsenvironmentid-delete
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: environmentId
        description: The GTM Environment ID
      responses:
        200:
          description: OK
      tags:
      - GTM Environment
    get:
      summary: Get GTM Environment
      description: Gets a GTM Environment.
      operationId: tagmanager.accounts.containers.environments.get
      x-api-path-slug: accountsaccountidcontainerscontaineridenvironmentsenvironmentid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: environmentId
        description: The GTM Environment ID
      responses:
        200:
          description: OK
      tags:
      - GTM Environment
    patch:
      summary: Update GTM Environment
      description: Updates a GTM Environment. This method supports patch semantics.
      operationId: tagmanager.accounts.containers.environments.patch
      x-api-path-slug: accountsaccountidcontainerscontaineridenvironmentsenvironmentid-patch
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: environmentId
        description: The GTM Environment ID
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the environment in storage
      responses:
        200:
          description: OK
      tags:
      - GTM Environment
    put:
      summary: Update GTM Environment
      description: Updates a GTM Environment.
      operationId: tagmanager.accounts.containers.environments.update
      x-api-path-slug: accountsaccountidcontainerscontaineridenvironmentsenvironmentid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: environmentId
        description: The GTM Environment ID
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the environment in storage
      responses:
        200:
          description: OK
      tags:
      - GTM Environment
  /accounts/{accountId}/containers/{containerId}/folders:
    get:
      summary: Get GTM Folders
      description: Lists all GTM Folders of a Container.
      operationId: tagmanager.accounts.containers.folders.list
      x-api-path-slug: accountsaccountidcontainerscontaineridfolders-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Folder
    post:
      summary: Create GTM Folder
      description: Creates a GTM Folder.
      operationId: tagmanager.accounts.containers.folders.create
      x-api-path-slug: accountsaccountidcontainerscontaineridfolders-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Folder
  /accounts/{accountId}/containers/{containerId}/folders/{folderId}:
    delete:
      summary: Delete GTM Folder
      description: Deletes a GTM Folder.
      operationId: tagmanager.accounts.containers.folders.delete
      x-api-path-slug: accountsaccountidcontainerscontaineridfoldersfolderid-delete
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: folderId
        description: The GTM Folder ID
      responses:
        200:
          description: OK
      tags:
      - GTM Folder
    get:
      summary: Get GTM Folder
      description: Gets a GTM Folder.
      operationId: tagmanager.accounts.containers.folders.get
      x-api-path-slug: accountsaccountidcontainerscontaineridfoldersfolderid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: folderId
        description: The GTM Folder ID
      responses:
        200:
          description: OK
      tags:
      - GTM Folder
    put:
      summary: Update GTM Folder
      description: Updates a GTM Folder.
      operationId: tagmanager.accounts.containers.folders.update
      x-api-path-slug: accountsaccountidcontainerscontaineridfoldersfolderid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the folder in storage
      - in: path
        name: folderId
        description: The GTM Folder ID
      responses:
        200:
          description: OK
      tags:
      - GTM Folder
  /accounts/{accountId}/containers/{containerId}/folders/{folderId}/entities:
    get:
      summary: Get Entities
      description: List all entities in a GTM Folder.
      operationId: tagmanager.accounts.containers.folders.entities.list
      x-api-path-slug: accountsaccountidcontainerscontaineridfoldersfolderidentities-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: folderId
        description: The GTM Folder ID
      responses:
        200:
          description: OK
      tags:
      - Entity
  /accounts/{accountId}/containers/{containerId}/move_folders/{folderId}:
    put:
      summary: Move Entity
      description: Moves entities to a GTM Folder.
      operationId: tagmanager.accounts.containers.move_folders.update
      x-api-path-slug: accountsaccountidcontainerscontaineridmove-foldersfolderid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: folderId
        description: The GTM Folder ID
      - in: query
        name: tagId
        description: The tags to be moved to the folder
      - in: query
        name: triggerId
        description: The triggers to be moved to the folder
      - in: query
        name: variableId
        description: The variables to be moved to the folder
      responses:
        200:
          description: OK
      tags:
      - Entity
  /accounts/{accountId}/containers/{containerId}/reauthorize_environments/{environmentId}:
    put:
      summary: Regenerate Authorization
      description: Re-generates the authorization code for a GTM Environment.
      operationId: tagmanager.accounts.containers.reauthorize_environments.update
      x-api-path-slug: accountsaccountidcontainerscontaineridreauthorize-environmentsenvironmentid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: environmentId
        description: The GTM Environment ID
      responses:
        200:
          description: OK
      tags:
      - Authorization
  /accounts/{accountId}/containers/{containerId}/tags:
    get:
      summary: Get GTM Tags
      description: Lists all GTM Tags of a Container.
      operationId: tagmanager.accounts.containers.tags.list
      x-api-path-slug: accountsaccountidcontainerscontaineridtags-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Tag
    post:
      summary: Create GTM Tag
      description: Creates a GTM Tag.
      operationId: tagmanager.accounts.containers.tags.create
      x-api-path-slug: accountsaccountidcontainerscontaineridtags-post
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      responses:
        200:
          description: OK
      tags:
      - GTM Tag
  /accounts/{accountId}/containers/{containerId}/tags/{tagId}:
    delete:
      summary: Delete GTM Tag
      description: Deletes a GTM Tag.
      operationId: tagmanager.accounts.containers.tags.delete
      x-api-path-slug: accountsaccountidcontainerscontaineridtagstagid-delete
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: tagId
        description: The GTM Tag ID
      responses:
        200:
          description: OK
      tags:
      - GTM Tag
    get:
      summary: Get GTM Tag
      description: Gets a GTM Tag.
      operationId: tagmanager.accounts.containers.tags.get
      x-api-path-slug: accountsaccountidcontainerscontaineridtagstagid-get
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: path
        name: tagId
        description: The GTM Tag ID
      responses:
        200:
          description: OK
      tags:
      - GTM Tag
    put:
      summary: Update GTM Tag
      description: Updates a GTM Tag.
      operationId: tagmanager.accounts.containers.tags.update
      x-api-path-slug: accountsaccountidcontainerscontaineridtagstagid-put
      parameters:
      - in: path
        name: accountId
        description: The GTM Account ID
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: containerId
        description: The GTM Container ID
      - in: query
        name: fingerprint
        description: When provided, this fingerprint must match the fingerprint of
          the tag in storage
      - in: path
        name: tagId
        description: The GTM Tag ID
      responses:
        200:
          description: OK
      tags:
      - GTM Tag
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