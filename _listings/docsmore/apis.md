---
name: Docsmore
x-slug: docsmore
description: FORM.FILL.SIGN - With Docsmore, the process of setting up a form and
  sending to users to complete or sign is simplified.  Use our platform to easily
  upload a document, specify form fields/signage, and send to users for completion.  Present
  forms to you...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28946-api-docsmore-com.jpg
x-kinRank: "7"
x-alexaRank: "7238418"
tags: Docsmore
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/apis.md
specificationVersion: "0.14"
apis:
- name: Docsmore API 2.1 - List all Webhooks
  x-api-slug: apigetwebhooks-get
  description: List Webhooks that are both active and inactive. Inactive webhooks
    with webhook type of 'static' will be automatically removed during the nightly
    job process.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28946-api-docsmore-com.jpg
  humanURL: http://api.docsmore.com
  baseURL: https://api.docsmore.com//
  tags: SaaS, Technology, Documents, Forms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/apigetwebhooks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/apigetwebhooks-get-openapi.md
- name: Docsmore API 2.1 - Unsubscribe Webhook
  x-api-slug: apiwebhookunsubscribeid-delete
  description: It is important that you call this event to unsubscribe otherwise it
    will automatically be removed in 10 minutes. If not unsubscribed manually, it
    can also lead to the problem of duplication and create further issues.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28946-api-docsmore-com.jpg
  humanURL: http://api.docsmore.com
  baseURL: https://api.docsmore.com//
  tags: SaaS, Technology, Documents, Forms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/apiwebhookunsubscribeid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/apiwebhookunsubscribeid-delete-openapi.md
- name: Docsmore API 2.1 - Fetch All Documents from Your Team Catalogue
  x-api-slug: apidmcatalogue-post
  description: By design, the authenticated user can only view the files that are
    either created by them or shared with them. Make sure user has at least read permission
    to view the catalogue.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28946-api-docsmore-com.jpg
  humanURL: http://api.docsmore.com
  baseURL: https://api.docsmore.com//
  tags: SaaS, Technology, Documents, Forms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/apidmcatalogue-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/apidmcatalogue-post-openapi.md
- name: Docsmore API 2.1 - Fetch Single Document
  x-api-slug: apidmcatalogueid-post
  description: Fetch single document.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28946-api-docsmore-com.jpg
  humanURL: http://api.docsmore.com
  baseURL: https://api.docsmore.com//
  tags: SaaS, Technology, Documents, Forms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/apidmcatalogueid-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/apidmcatalogueid-post-openapi.md
- name: Docsmore API 2.1 - Get All Document Flows
  x-api-slug: apidocflowgetdocflows-get
  description: Get all document flows.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28946-api-docsmore-com.jpg
  humanURL: http://api.docsmore.com
  baseURL: https://api.docsmore.com//
  tags: SaaS, Technology, Documents, Forms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/apidocflowgetdocflows-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/apidocflowgetdocflows-get-openapi.md
- name: Docsmore API 2.1 - Get Raw Data For A Given Document
  x-api-slug: apiclientdocsgetrawdataauthtokendocumentkey-get
  description: |-
    This API call gets you underlying raw data of the document. All you need to do is supply Auth token and Document Key as part of the call.

    Document Key can be obtained from "Document Gallery" Page and Clicking on the sub-menu of the desired document.

    As a response object, jsondata and metadata information is passed. Jsondata is basically raw data and metadata is data columns information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28946-api-docsmore-com.jpg
  humanURL: http://api.docsmore.com
  baseURL: https://api.docsmore.com//
  tags: SaaS, Technology, Documents, Forms
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/apiclientdocsgetrawdataauthtokendocumentkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/apiclientdocsgetrawdataauthtokendocumentkey-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://digitalocean.api.gallery.streamdata.io
- type: x-email
  url: contact@docsmore.com
- type: x-twitter
  url: https://twitter.com/docsmore
- type: x-website
  url: http://api.docsmore.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---