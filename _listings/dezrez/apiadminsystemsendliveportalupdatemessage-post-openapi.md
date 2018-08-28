---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: "Dezrez Sends a message to the LivePortalJobHandler that says \r\nthe specified
    property marketing role has changed"
  version: 1.0.0
  description: "Sends a message to the liveportaljobhandler that says \r\nthe specified
    property marketing role has changed."
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/admin/portal/getportaluploadsforrole:
    get:
      summary: Get all the live portal uploads associated with a property marketing
        role
      description: Get all the live portal uploads associated with a property marketing
        role.
      operationId: Portal_GetLivePortalInformationRecordsForRoleByroleId
      x-api-path-slug: apiadminportalgetportaluploadsforrole-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Live
      - Portal
      - Uploads
      - Associated
      - Property
      - Marketing
      - Role
  /api/admin/system/sendNotificationToAllUsersInAgency:
    post:
      summary: Send a live notification to all active users in an agency
      description: Send a live notification to all active users in an agency.
      operationId: System_SendNotificationToAgencyUsersByagencyIdBysendNotification
      x-api-path-slug: apiadminsystemsendnotificationtoallusersinagency-post
      parameters:
      - in: query
        name: agencyId
        description: The agency identifier
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: sendNotification
        description: The send notification
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Send
      - Live
      - Notification
      - To
      - ""
      - Active
      - Users
      - In
      - Agency
  /api/admin/system/sendliveportalupdatemessage:
    post:
      summary: "Sends a message to the LivePortalJobHandler that says \r\nthe specified
        property marketing role has changed"
      description: "Sends a message to the liveportaljobhandler that says \r\nthe
        specified property marketing role has changed."
      operationId: System_SendLivePortalUpdateMessageBypropertyMarketingRoleId
      x-api-path-slug: apiadminsystemsendliveportalupdatemessage-post
      parameters:
      - in: query
        name: propertyMarketingRoleId
        description: The property marketing role ID
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sends
      - Message
      - To
      - LivePortalJobHandler
      - That
      - Says
      - The
      - Specified
      - Property
      - Marketing
      - Role
      - Has
      - Changed
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