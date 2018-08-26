---
swagger: "2.0"
x-collection-name: AWS Cognito
x-complete: 1
info:
  title: AWS Cognito Merged API
  version: 1.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=GetCSVHeader:
    get:
      summary: Get C S V Header
      description: Gets the header information for the.
      operationId: getCSVHeader
      x-api-path-slug: actiongetcsvheader-get
      parameters:
      - in: query
        name: UserPoolId
        description: The user pool ID for the user pool that the users are to be imported            into
        type: string
      responses:
        200:
          description: OK
      tags:
      - CSV Header
---