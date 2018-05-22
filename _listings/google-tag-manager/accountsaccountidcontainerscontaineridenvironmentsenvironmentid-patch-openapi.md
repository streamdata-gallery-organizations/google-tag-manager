---
swagger: "2.0"
x-collection-name: Google Tag Manager
x-complete: 0
info:
  title: Google Tag Manager API Update GTM Environment
  description: Updates a GTM Environment. This method supports patch semantics.
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