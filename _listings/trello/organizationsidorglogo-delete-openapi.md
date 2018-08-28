---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Delete Organizations Logo
  description: Delete organizations logo.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/{idOrg}/logo:
    delete:
      summary: Delete Organizations Logo
      description: Delete organizations logo.
      operationId: deleteOrganizationsLogoByIdOrg
      x-api-path-slug: organizationsidorglogo-delete
      parameters:
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Logo
    post:
      summary: Post Organizations Logo
      description: Post organizations logo.
      operationId: addOrganizationsLogoByIdOrg
      x-api-path-slug: organizationsidorglogo-post
      parameters:
      - in: body
        name: body
        description: Attributes of Organizations Logo to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idOrg
        description: idOrg or name
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Logo
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