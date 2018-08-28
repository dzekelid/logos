---
swagger: "2.0"
x-collection-name: Lykke
x-complete: 0
info:
  title: Lykke Add API Auth Logout
  version: 1.0.0
  description: Add api auth logout.
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/Auth/LogOut:
    post:
      summary: Add API Auth Logout
      description: Add api auth logout.
      operationId: ApiAuthLogOutPost
      x-api-path-slug: apiauthlogout-post
      parameters:
      - in: header
        name: Authorization
        description: access token
      responses:
        200:
          description: OK
      tags:
      - Auth
      - Logout
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