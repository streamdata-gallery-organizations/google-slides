---
swagger: "2.0"
x-collection-name: Google Slides
x-complete: 0
info:
  title: Google Slides API Get Presentation
  description: Gets the latest version of the specified presentation.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: slides.googleapis.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/presentations:
    post:
      summary: Create Presentation
      description: |-
        Creates a new presentation using the title given in the request. Other
        fields in the request are ignored.
        Returns the created presentation.
      operationId: slides.presentations.create
      x-api-path-slug: v1presentations-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Presentation
  /v1/presentations/{presentationId}:
    get:
      summary: Get Presentation
      description: Gets the latest version of the specified presentation.
      operationId: slides.presentations.get
      x-api-path-slug: v1presentationspresentationid-get
      parameters:
      - in: path
        name: presentationId
        description: The ID of the presentation to retrieve
      responses:
        200:
          description: OK
      tags:
      - Presentation
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