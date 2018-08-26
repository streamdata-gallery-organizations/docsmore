---
swagger: "2.0"
x-collection-name: Docsmore
x-complete: 0
info:
  title: Docsmore Unsubscribe Webhook
  description: It is important that you call this event to unsubscribe otherwise it
    will automatically be removed in 10 minutes. If not unsubscribed manually, it
    can also lead to the problem of duplication and create further issues.
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