---
swagger: "2.0"
x-collection-name: EhrScape
x-complete: 0
info:
  title: Ehr Scape Electronic Health Record APIs Import CSV data.
  description: Import csv data..
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
host: rest.ehrscape.com
basePath: /rest/v1
paths:
  /import/csv:
    post:
      summary: Import CSV data.
      description: Import csv data..
      operationId: importData
      x-api-path-slug: importcsv-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: committerName
        description: Committer name (if not specified username is used instead)
      - in: query
        name: composerName
        description: Composer name (if not specified username is used instead)
      - in: query
        name: converterLocale
        description: Converter locale - specify when numeric values are formatted
          in a specific locale
      - in: query
        name: subjectNamespace
        description: Subject namespace (required when using subjectIds to identify
          EHRs)
      - in: query
        name: templateId
        description: Template ID
      - in: query
        name: templateLanguage
        description: Template language
      responses:
        200:
          description: OK
      tags:
      - Import
      - Csv
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