---
swagger: "2.0"
x-collection-name: Google Doubleclick
x-complete: 0
info:
  title: Google Doubleclick API Upload CSV
  version: 1.0.0
  description: Uploads line items in CSV format.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lineitems/downloadlineitems:
    post:
      summary: Download CSV
      description: Retrieves line items in CSV format.
      operationId: doubleclickbidmanager.lineitems.downloadlineitems
      x-api-path-slug: lineitemsdownloadlineitems-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - CSV
  /lineitems/uploadlineitems:
    post:
      summary: Upload CSV
      description: Uploads line items in CSV format.
      operationId: doubleclickbidmanager.lineitems.uploadlineitems
      x-api-path-slug: lineitemsuploadlineitems-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Advertising
      - CSV
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