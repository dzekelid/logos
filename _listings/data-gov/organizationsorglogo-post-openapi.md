---
swagger: "2.0"
x-collection-name: Data.Gov
x-complete: 0
info:
  title: Data.gov API Add Organizations Org Logo
  description: Upload a new logo
  version: "3"
host: catalog.data.gov
basePath: /api/3/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /organizations/{org}/logo:
    post:
      summary: Add Organizations Org Logo
      description: Upload a new logo
      operationId: postOrganizationsOrgLogo
      x-api-path-slug: organizationsorglogo-post
      parameters:
      - in: formData
        name: bbox
      - in: formData
        name: file
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
      - Logo
    put:
      summary: Put Organizations Org Logo
      description: Set the logo BBox
      operationId: putOrganizationsOrgLogo
      x-api-path-slug: organizationsorglogo-put
      parameters:
      - in: formData
        name: bbox
      - in: formData
        name: file
      - in: path
        name: org
        description: The organization ID or slug
      responses:
        200:
          description: OK
      tags:
      - Organizations
      - Org
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