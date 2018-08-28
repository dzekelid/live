---
swagger: "2.0"
x-collection-name: Postmark
x-complete: 1
info:
  title: Postmark
  description: send-emails-retrieve-bounces-and-start-accepting-inbound-emails-all-via-an-easytouse-http-api-
  version: 1.0.0
host: spamcheck.postmarkapp.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /deliverystats:
    parameters:
      summary: Parameters Deliverystats
      description: Parameters deliverystats.
      operationId: parametersDeliverystats
      x-api-path-slug: deliverystats-parameters
      responses:
        200:
          description: OK
      tags:
      - Deliverystats
    get:
      summary: Get Deliverystats
      description: Returns a summary of inactive emails and bounces by type.
      operationId: getDeliverystats
      x-api-path-slug: deliverystats-get
      parameters:
      - in: query
        name: Accept
        description: The accepted type for the response
      - in: query
        name: Content-Type
        description: The content type of the request
      - in: header
        name: X-Postmark-Server-Token
        description: The token associated with the Server on which this request will
          operate
      responses:
        200:
          description: OK
      tags:
      - Deliverystats
---