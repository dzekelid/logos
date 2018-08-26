---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 1
info:
  title: GIG & Crowd
  version: 1.0.0
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/account/logout:
    post:
      summary: Post Account Logout
      description: Post account logout.
      operationId: postApiV1AccountLogout
      x-api-path-slug: apiv1accountlogout-post
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Account
      - Logout
---