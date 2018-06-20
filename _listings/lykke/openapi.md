---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 1
info:
  title: Wallet_Api
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/IsAlive:
    get:
      summary: Get API Isalive
      description: Get api isalive.
      operationId: ApiIsAliveGet
      x-api-path-slug: apiisalive-get
      responses:
        200:
          description: OK
      tags:
      - Isalive
---