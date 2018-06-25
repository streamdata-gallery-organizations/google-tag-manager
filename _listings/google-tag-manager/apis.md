---
name: Google Tag Manager
x-slug: google-tag-manager
description: Deploy and update measurement tags on your websites and mobile apps without
  major code changes and app releases. Use Google Tag Manager to manage tags (such
  as tracking and marketing optimization JavaScript tags) on your site. Without editing
  your site code, you use GTM user interface to add and update AdWords, Google Analytics,
  Floodlight, and non-Google tags. This reduces errors and allows you to to deploy
  tags on your site quickly.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Google Tag Manager
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/apis.md
specificationVersion: "0.14"
apis:
- name: Google Tag Manager API Get Accounts
  x-api-slug: google-tag-manager-api
  description: Lists all GTM Accounts that a user has access to.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts
  tags: Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accounts-get-openapi.md
- name: Google Tag Manager API Get Account
  x-api-slug: google-tag-manager-api
  description: Gets a GTM Account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}
  tags: Account
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountid-get-openapi.md
- name: Google Tag Manager API Update Account
  x-api-slug: google-tag-manager-api
  description: Updates a GTM Account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}
  tags: Account
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountid-put-openapi.md
- name: Google Tag Manager API Get Conainers
  x-api-slug: google-tag-manager-api
  description: Lists all Containers that belongs to a GTM Account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers
  tags: Container
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainers-get-openapi.md
- name: Google Tag Manager API Create Container
  x-api-slug: google-tag-manager-api
  description: Creates a Container.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers
  tags: Container
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainers-post-openapi.md
- name: Google Tag Manager API Delete Container
  x-api-slug: google-tag-manager-api
  description: Deletes a Container.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}
  tags: Container
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontainerid-delete-openapi.md
- name: Google Tag Manager API Get Container
  x-api-slug: google-tag-manager-api
  description: Gets a Container.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}
  tags: Container
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontainerid-get-openapi.md
- name: Google Tag Manager API Update Container
  x-api-slug: google-tag-manager-api
  description: Updates a Container.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}
  tags: Container
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontainerid-put-openapi.md
- name: Google Tag Manager API Get GTM Environments
  x-api-slug: google-tag-manager-api
  description: Lists all GTM Environments of a GTM Container.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/environments
  tags: GTM Environment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridenvironments-get-openapi.md
- name: Google Tag Manager API Create GTM Environment
  x-api-slug: google-tag-manager-api
  description: Creates a GTM Environment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/environments
  tags: GTM Environment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridenvironments-post-openapi.md
- name: Google Tag Manager API Delete GTM Environment
  x-api-slug: google-tag-manager-api
  description: Deletes a GTM Environment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/environments/{environmentId}
  tags: GTM Environment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridenvironmentsenvironmentid-delete-openapi.md
- name: Google Tag Manager API Get GTM Environment
  x-api-slug: google-tag-manager-api
  description: Gets a GTM Environment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/environments/{environmentId}
  tags: GTM Environment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridenvironmentsenvironmentid-get-openapi.md
- name: Google Tag Manager API Update GTM Environment
  x-api-slug: google-tag-manager-api
  description: Updates a GTM Environment. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/environments/{environmentId}
  tags: GTM Environment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridenvironmentsenvironmentid-patch-openapi.md
- name: Google Tag Manager API Update GTM Environment
  x-api-slug: google-tag-manager-api
  description: Updates a GTM Environment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/environments/{environmentId}
  tags: GTM Environment
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridenvironmentsenvironmentid-put-openapi.md
- name: Google Tag Manager API Get GTM Folders
  x-api-slug: google-tag-manager-api
  description: Lists all GTM Folders of a Container.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/folders
  tags: GTM Folder
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridfolders-get-openapi.md
- name: Google Tag Manager API Create GTM Folder
  x-api-slug: google-tag-manager-api
  description: Creates a GTM Folder.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/folders
  tags: GTM Folder
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridfolders-post-openapi.md
- name: Google Tag Manager API Delete GTM Folder
  x-api-slug: google-tag-manager-api
  description: Deletes a GTM Folder.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/folders/{folderId}
  tags: GTM Folder
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridfoldersfolderid-delete-openapi.md
- name: Google Tag Manager API Get GTM Folder
  x-api-slug: google-tag-manager-api
  description: Gets a GTM Folder.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/folders/{folderId}
  tags: GTM Folder
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridfoldersfolderid-get-openapi.md
- name: Google Tag Manager API Update GTM Folder
  x-api-slug: google-tag-manager-api
  description: Updates a GTM Folder.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/folders/{folderId}
  tags: GTM Folder
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridfoldersfolderid-put-openapi.md
- name: Google Tag Manager API Get Entities
  x-api-slug: google-tag-manager-api
  description: List all entities in a GTM Folder.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/folders/{folderId}/entities
  tags: Entity
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridfoldersfolderidentities-get-openapi.md
- name: Google Tag Manager API Move Entity
  x-api-slug: google-tag-manager-api
  description: Moves entities to a GTM Folder.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/move_folders/{folderId}
  tags: Entity
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridmove-foldersfolderid-put-openapi.md
- name: Google Tag Manager API Regenerate Authorization
  x-api-slug: google-tag-manager-api
  description: Re-generates the authorization code for a GTM Environment.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/reauthorize_environments/{environmentId}
  tags: Authorization
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridreauthorize-environmentsenvironmentid-put-openapi.md
- name: Google Tag Manager API Get GTM Tags
  x-api-slug: google-tag-manager-api
  description: Lists all GTM Tags of a Container.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/tags
  tags: GTM Tag
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridtags-get-openapi.md
- name: Google Tag Manager API Create GTM Tag
  x-api-slug: google-tag-manager-api
  description: Creates a GTM Tag.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/tags
  tags: GTM Tag
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridtags-post-openapi.md
- name: Google Tag Manager API Delete GTM Tag
  x-api-slug: google-tag-manager-api
  description: Deletes a GTM Tag.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/tags/{tagId}
  tags: GTM Tag
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridtagstagid-delete-openapi.md
- name: Google Tag Manager API Get GTM Tag
  x-api-slug: google-tag-manager-api
  description: Gets a GTM Tag.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/tags/{tagId}
  tags: GTM Tag
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridtagstagid-get-openapi.md
- name: Google Tag Manager API Update GTM Tag
  x-api-slug: google-tag-manager-api
  description: Updates a GTM Tag.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/tags/{tagId}
  tags: GTM Tag
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridtagstagid-put-openapi.md
- name: Google Tag Manager API Get GTM Triggers
  x-api-slug: google-tag-manager-api
  description: Lists all GTM Triggers of a Container.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/triggers
  tags: GTM Trigger
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridtriggers-get-openapi.md
- name: Google Tag Manager API Create GTM Trigger
  x-api-slug: google-tag-manager-api
  description: Creates a GTM Trigger.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/triggers
  tags: GTM Trigger
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridtriggers-post-openapi.md
- name: Google Tag Manager API Delete GTM Trigger
  x-api-slug: google-tag-manager-api
  description: Deletes a GTM Trigger.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/triggers/{triggerId}
  tags: GTM Trigger
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridtriggerstriggerid-delete-openapi.md
- name: Google Tag Manager API Get GTM Trigger
  x-api-slug: google-tag-manager-api
  description: Gets a GTM Trigger.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/triggers/{triggerId}
  tags: GTM Trigger
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridtriggerstriggerid-get-openapi.md
- name: Google Tag Manager API Update GTM Trigger
  x-api-slug: google-tag-manager-api
  description: Updates a GTM Trigger.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/triggers/{triggerId}
  tags: GTM Trigger
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridtriggerstriggerid-put-openapi.md
- name: Google Tag Manager API Get GTM Variables
  x-api-slug: google-tag-manager-api
  description: Lists all GTM Variables of a Container.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/variables
  tags: GTM Variable
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridvariables-get-openapi.md
- name: Google Tag Manager API Create GTM Variable
  x-api-slug: google-tag-manager-api
  description: Creates a GTM Variable.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/variables
  tags: GTM Variable
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridvariables-post-openapi.md
- name: Google Tag Manager API Delete GTM Variable
  x-api-slug: google-tag-manager-api
  description: Deletes a GTM Variable.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/variables/{variableId}
  tags: GTM Variable
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridvariablesvariableid-delete-openapi.md
- name: Google Tag Manager API Get GTM Variable
  x-api-slug: google-tag-manager-api
  description: Gets a GTM Variable.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/variables/{variableId}
  tags: GTM Variable
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridvariablesvariableid-get-openapi.md
- name: Google Tag Manager API Update GTM Variable
  x-api-slug: google-tag-manager-api
  description: Updates a GTM Variable.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/variables/{variableId}
  tags: GTM Variable
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridvariablesvariableid-put-openapi.md
- name: Google Tag Manager API Get Container Versions
  x-api-slug: google-tag-manager-api
  description: Lists all Container Versions of a GTM Container.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/versions
  tags: Containers,Versions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversions-get-openapi.md
- name: Google Tag Manager API Create Container Version
  x-api-slug: google-tag-manager-api
  description: Creates a Container Version.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/versions
  tags: Containers,Versions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversions-post-openapi.md
- name: Google Tag Manager API Delete Container Version
  x-api-slug: google-tag-manager-api
  description: Deletes a Container Version.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}
  tags: Containers,Versions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionid-delete-openapi.md
- name: Google Tag Manager API Get Container Version
  x-api-slug: google-tag-manager-api
  description: Gets a Container Version.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}
  tags: Containers,Versions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionid-get-openapi.md
- name: Google Tag Manager API Update Container Version
  x-api-slug: google-tag-manager-api
  description: Updates a Container Version.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}
  tags: Containers,Versions
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionid-put-openapi.md
- name: Google Tag Manager API Publish Container Version
  x-api-slug: google-tag-manager-api
  description: Publishes a Container Version.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}/publish
  tags: Containers,Versions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionidpublish-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionidpublish-post-openapi.md
- name: Google Tag Manager API Restore Container Version
  x-api-slug: google-tag-manager-api
  description: Restores a Container Version. This will overwrite the container's current
    configuration (including its variables, triggers and tags). The operation will
    not have any effect on the version that is being served (i.e. the published version).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}/restore
  tags: Containers,Versions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionidrestore-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionidrestore-post-openapi.md
- name: Google Tag Manager API Undelete Container Version
  x-api-slug: google-tag-manager-api
  description: Undeletes a Container Version.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/containers/{containerId}/versions/{containerVersionId}/undelete
  tags: Containers,Versions
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionidundelete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidcontainerscontaineridversionscontainerversionidundelete-post-openapi.md
- name: Google Tag Manager API Get User Permissions
  x-api-slug: google-tag-manager-api
  description: List all users that have access to the account along with Account and
    Container Permissions granted to each of them.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/permissions
  tags: User Permission
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidpermissions-get-openapi.md
- name: Google Tag Manager API Create User Permission
  x-api-slug: google-tag-manager-api
  description: Creates a user's Account & Container Permissions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/permissions
  tags: User Permission
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidpermissions-post-openapi.md
- name: Google Tag Manager API Remove User
  x-api-slug: google-tag-manager-api
  description: Removes a user from the account, revoking access to it and all of its
    containers.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/permissions/{permissionId}
  tags: User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidpermissionspermissionid-delete-openapi.md
- name: Google Tag Manager API Get User
  x-api-slug: google-tag-manager-api
  description: Gets a user's Account & Container Permissions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/permissions/{permissionId}
  tags: User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidpermissionspermissionid-get-openapi.md
- name: Google Tag Manager API Update User
  x-api-slug: google-tag-manager-api
  description: Updates a user's Account & Container Permissions.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1//accounts/{accountId}/permissions/{permissionId}
  tags: User
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/accountsaccountidpermissionspermissionid-put-openapi.md
- name: Google Tag Manager API
  x-api-slug: google-tag-manager-api
  description: Deploy and update measurement tags on your websites and mobile apps
    without major code changes and app releases. Use Google Tag Manager to manage
    tags (such as tracking and marketing optimization JavaScript tags) on your site.
    Without editing your site code, you use GTM user interface to add and update AdWords,
    Google Analytics, Floodlight, and non-Google tags. This reduces errors and allows
    you to to deploy tags on your site quickly.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/googl_tag_manager_gplus-250.png
  humanURL: https://developers.google.com/tag-manager/
  baseURL: ://www.googleapis.com//tagmanager/v1
  tags: Google Tag Manager
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/google-tag-manager/master/_listings/google-tag-manager/openapi.md
x-common:
- type: x-authentication
  url: https://developers.google.com/tag-manager/api/v1/authorization
- type: x-change-log
  url: https://developers.google.com/tag-manager/api/v1/changelog
- type: x-code
  url: https://developers.google.com/tag-manager/api/v1/libraries
- type: x-documentation
  url: https://developers.google.com/tag-manager/api/v1/
- type: x-performance
  url: https://developers.google.com/tag-manager/api/v1/performance
- type: x-website
  url: https://developers.google.com/tag-manager/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---