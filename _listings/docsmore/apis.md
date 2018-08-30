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
created: "2018-08-30"
modified: "2018-08-30"
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
- name: Docsmore API 2.1 - Get Details of Single Webhook
  x-api-slug: apigetwebhooksid-get
  description: Details of Single Webhook.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28946-api-docsmore-com.jpg
  humanURL: http://api.docsmore.com
  baseURL: https://api.docsmore.com//
  tags: SaaS, Technology, Documents, Forms
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/apigetwebhooksid-get-openapi.md
- name: Docsmore API 2.1 - Subscribe To Webhook
  x-api-slug: apiwebhooksubscribe-post
  description: |-
    Make sure you have a unique payload URL every time you use this api call to register your webhook. Unable to do so will result in webhook registration denial.


    For multiple events subscription, just use it comma separated values. Here are the available list of register events.



    documentUploadComplete
    workflowProgressEvent
    workflowCompleteEvent
    documentflowProgressEvent
    documentflowCompleteEvent
    documentSelfSigninCompleteEvent
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28946-api-docsmore-com.jpg
  humanURL: http://api.docsmore.com
  baseURL: https://api.docsmore.com//
  tags: SaaS, Technology, Documents, Forms
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/apiwebhooksubscribe-post-openapi.md
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
- name: Docsmore API 2.1 - Get OAuth TOKEN
  x-api-slug: oauthtoken-post
  description: |-
    Obtaining an Auth Token is the first thing in the process. The lifetime of Auth token is configurable in the developer portal depending upon your need. Once auth token is obtained, all the follow up API calls will need to include auth token in the header. FaIlure to do so would result in response with 401 Unauthorized Access.

    Under Your Developer Account - Go to Api Setting and you will screen similar to below.


    Make sure you call this in server side code. Exposing apiKey and clientSecret is a not a good idea on front end and can lead up to security vulnerabilities.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28946-api-docsmore-com.jpg
  humanURL: http://api.docsmore.com
  baseURL: https://api.docsmore.com//
  tags: SaaS, Technology, Documents, Forms
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/oauthtoken-post-openapi.md
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
- name: Docsmore API 2.1 - Get Workflow Link
  x-api-slug: apigetworkflowlink-post
  description: |-
    This is the most popular use of Docsmore API. From your connected app, you can launch workflow and obtain the unique link for immediate launch or later on. You can also supply data in flat json format that can be used inside the document for pre-fill purpose saving your customer time.

    Please make sure you pay close attention to the requirement for this API call as there are several aspects of it as required parameters.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28946-api-docsmore-com.jpg
  humanURL: http://api.docsmore.com
  baseURL: https://api.docsmore.com//
  tags: SaaS, Technology, Documents, Forms
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/apigetworkflowlink-post-openapi.md
- name: Docsmore API 2.1 - Get Workflow Link For Flow Track
  x-api-slug: apidocflowtracksflowtrackviaapi-post
  description: |-
    In Docsmore space, Flow Track means all the client documents generated using one of the Document Flow. In other words, it is an instance of Document FLow. The other thing to notice here is payload information is remarkably similar to general "Workflow" of a Single Document.

    When you initiate this API call, you are basically setting up a new instance of Workflow and in turn getting workflow link of the starting document in the workflow.

    If "flowtrackid" value is "new", then new flowtrack will be created. If flowtrackid has a value of actual flowtrackid then link will be provided to access read-only view of document flowtrack
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28946-api-docsmore-com.jpg
  humanURL: http://api.docsmore.com
  baseURL: https://api.docsmore.com//
  tags: SaaS, Technology, Documents, Forms
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/apidocflowtracksflowtrackviaapi-post-openapi.md
- name: Docsmore API 2.1 - Returns raw data response as json FOR SINGLE CLIENT DOC
  x-api-slug: rawdata-post
  description: This API call gets you underlying raw data of the document. All you
    need to do is supply Auth token and Document Key as part of the call
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28946-api-docsmore-com.jpg
  humanURL: http://api.docsmore.com
  baseURL: https://api.docsmore.com//
  tags: SaaS, Technology, Documents, Forms
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/rawdata-post-openapi.md
- name: Docsmore API 2.1 - Get List of Client Documents By Document ID
  x-api-slug: getclientdocs-post
  description: In order to export as PDf, you will need to have client document ID
    available for that specific document you are looking to download.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28946-api-docsmore-com.jpg
  humanURL: http://api.docsmore.com
  baseURL: https://api.docsmore.com//
  tags: SaaS, Technology, Documents, Forms
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/getclientdocs-post-openapi.md
- name: Docsmore API 2.1 - Export As PDF
  x-api-slug: clientdocsexportpdfid-get
  description: In order to export as PDf, you will need to have client document ID
    available for that specific document you are looking to download.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/28946-api-docsmore-com.jpg
  humanURL: http://api.docsmore.com
  baseURL: https://api.docsmore.com//
  tags: SaaS, Technology, Documents, Forms
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/docsmore/master/_listings/docsmore/clientdocsexportpdfid-get-openapi.md
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