---
swagger: "2.0"
x-collection-name: Docsmore
x-complete: 0
info:
  title: Docsmore Get Workflow Link
  description: |-
    This is the most popular use of Docsmore API. From your connected app, you can launch workflow and obtain the unique link for immediate launch or later on. You can also supply data in flat json format that can be used inside the document for pre-fill purpose saving your customer time.

    Please make sure you pay close attention to the requirement for this API call as there are several aspects of it as required parameters.
  version: "1.0"
host: api.docsmore.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/getwebhooks:
    get:
      summary: List all Webhooks
      description: List Webhooks that are both active and inactive. Inactive webhooks
        with webhook type of 'static' will be automatically removed during the nightly
        job process.
      operationId: ApiGetwebhooksGet
      x-api-path-slug: apigetwebhooks-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Webhooks
  /api/getwebhooks/{id}:
    get:
      summary: Get Details of Single Webhook
      description: Details of Single Webhook.
      operationId: ApiGetwebhooksByIdGet
      x-api-path-slug: apigetwebhooksid-get
      parameters:
      - in: header
        name: Content-Type
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Details
      - Of
      - Single
      - Webhook
  /api/webhook/subscribe:
    post:
      summary: Subscribe To Webhook
      description: |-
        Make sure you have a unique payload URL every time you use this api call to register your webhook. Unable to do so will result in webhook registration denial.


        For multiple events subscription, just use it comma separated values. Here are the available list of register events.



        documentUploadComplete
        workflowProgressEvent
        workflowCompleteEvent
        documentflowProgressEvent
        documentflowCompleteEvent
        documentSelfSigninCompleteEvent
      operationId: ApiWebhookSubscribePost
      x-api-path-slug: apiwebhooksubscribe-post
      parameters:
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Subscribe
      - Webhook
  /api/webhook/unsubscribe/{id}:
    delete:
      summary: Unsubscribe Webhook
      description: It is important that you call this event to unsubscribe otherwise
        it will automatically be removed in 10 minutes. If not unsubscribed manually,
        it can also lead to the problem of duplication and create further issues.
      operationId: ApiWebhookUnsubscribeByIdDelete
      x-api-path-slug: apiwebhookunsubscribeid-delete
      parameters:
      - in: header
        name: Content-Type
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - Unsubscribe
      - Webhook
  /oauth/token:
    post:
      summary: Get OAuth TOKEN
      description: |-
        Obtaining an Auth Token is the first thing in the process. The lifetime of Auth token is configurable in the developer portal depending upon your need. Once auth token is obtained, all the follow up API calls will need to include auth token in the header. FaIlure to do so would result in response with 401 Unauthorized Access.

        Under Your Developer Account - Go to Api Setting and you will screen similar to below.


        Make sure you call this in server side code. Exposing apiKey and clientSecret is a not a good idea on front end and can lead up to security vulnerabilities.
      operationId: OauthTokenPost
      x-api-path-slug: oauthtoken-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - OAuth
      - TOKEN
  /api/dmcatalogue:
    post:
      summary: Fetch All Documents from Your Team Catalogue
      description: By design, the authenticated user can only view the files that
        are either created by them or shared with them. Make sure user has at least
        read permission to view the catalogue.
      operationId: ApiDmcataloguePost
      x-api-path-slug: apidmcatalogue-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: items
      - in: query
        name: page
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - ""
      - Documents
      - From
      - Your
      - Team
      - Catalogue
  /api/dmcatalogue/:id:
    post:
      summary: Fetch Single Document
      description: Fetch single document.
      operationId: ApiDmcatalogueIdPost
      x-api-path-slug: apidmcatalogueid-post
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: id
      responses:
        200:
          description: OK
      tags:
      - Fetch
      - Single
      - Document
  /api/docflow/getdocflows:
    get:
      summary: Get All Document Flows
      description: Get all document flows.
      operationId: ApiDocflowGetdocflowsGet
      x-api-path-slug: apidocflowgetdocflows-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Document
      - Flows
  /api/clientdocs/getrawdata/:authToken/:documentKey:
    get:
      summary: Get Raw Data For A Given Document
      description: |-
        This API call gets you underlying raw data of the document. All you need to do is supply Auth token and Document Key as part of the call.

        Document Key can be obtained from "Document Gallery" Page and Clicking on the sub-menu of the desired document.

        As a response object, jsondata and metadata information is passed. Jsondata is basically raw data and metadata is data columns information.
      operationId: ApiClientdocsGetrawdataAuthTokenDocumentKeyGet
      x-api-path-slug: apiclientdocsgetrawdataauthtokendocumentkey-get
      parameters:
      - in: header
        name: Accept
      - in: query
        name: authToken
      - in: header
        name: Content-Type
      - in: query
        name: documentKey
      responses:
        200:
          description: OK
      tags:
      - Raw
      - Data
      - Given
      - Document
  /api/getworkflowlink:
    post:
      summary: Get Workflow Link
      description: |-
        This is the most popular use of Docsmore API. From your connected app, you can launch workflow and obtain the unique link for immediate launch or later on. You can also supply data in flat json format that can be used inside the document for pre-fill purpose saving your customer time.

        Please make sure you pay close attention to the requirement for this API call as there are several aspects of it as required parameters.
      operationId: ApiGetworkflowlinkPost
      x-api-path-slug: apigetworkflowlink-post
      parameters:
      - in: header
        name: Accept
      - in: body
        name: Body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Workflow
      - Link
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