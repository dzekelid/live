---
swagger: "2.0"
x-collection-name: Zencoder
x-complete: 0
info:
  title: Zencoder API Get Usage for Live
  version: v2
  description: Get Usage for Live
host: app.zencoder.com
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /account/live:
    put:
      summary: Integration Mode - Live
      description: Integration Mode - Live
      operationId: putAccountLive
      x-api-path-slug: accountlive-put
      responses:
        200:
          description: OK
      tags:
      - Account
      - Live
  /reports/live:
    get:
      summary: Get Usage for Live
      description: Get Usage for Live
      operationId: getReportsLive
      x-api-path-slug: reportslive-get
      parameters:
      - in: query
        name: api_key
        description: The API key
      - in: query
        name: from
        description: 'Start date in the format YYYY-MM-DD (default: 30 days ago)'
      - in: query
        name: grouping
        description: 'Hour usage for only one report grouping (default: none)'
      - in: query
        name: to
        description: 'End date in the format YYYY-MM-DD (default: yesterday)'
      responses:
        200:
          description: OK
      tags:
      - Reports
      - Live
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