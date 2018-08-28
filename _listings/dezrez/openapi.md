swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
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