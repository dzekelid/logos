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
---