---
swagger: "2.0"
x-collection-name: Starred
x-complete: 0
info:
  title: Starred Send Invitation CSV
  description: "With the /sendinvitations call you can link your CRM system to Starred
    so invitations are sent automatically. This will no longer require any manual
    action. \n\nYou can also import additional characteristics directly from your
    CRM so you can start analyzing results for different client groups. \n\nThe parameters
    on the right are mandatory to make the request succeed.\n\n### Request Parameters\n\n|
    Parameter | Required | Description |\n| ------ | ------ | ------ |\n| `form` |
    Required | ID of the form that will be sent out |\n| `from` | Required | Email
    address of the sender, must be a registered email |\n| `template` | Required |
    Template ID |\n| `language` | Required | The language of the template. For example:
    nl, en or fr |\n| `file` | Required | A CSV file formatted as a regular invitation
    CSV added as a HTTP POST file. |\n| `reminder` | Optional | Whether or not to
    send a reminder (1 means On, 0 means Off). Defaults to 1 |\n\n### Example curl
    request\n```\ncurl -F \"file=@testCSV.csv\" https://api.starred.com/sendinvitations\\?company\\={{companyID}}\\&auth\\={{auth}}\\&form\\={{formId}}\\&from\\={{sender}}\\&template\\={{templateId}}\\&language\\={{language}}\n```"
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /sendinvitations/csv:
    post:
      summary: Send Invitation CSV
      description: "With the /sendinvitations call you can link your CRM system to
        Starred so invitations are sent automatically. This will no longer require
        any manual action. \n\nYou can also import additional characteristics directly
        from your CRM so you can start analyzing results for different client groups.
        \n\nThe parameters on the right are mandatory to make the request succeed.\n\n###
        Request Parameters\n\n| Parameter | Required | Description |\n| ------ | ------
        | ------ |\n| `form` | Required | ID of the form that will be sent out |\n|
        `from` | Required | Email address of the sender, must be a registered email
        |\n| `template` | Required | Template ID |\n| `language` | Required | The
        language of the template. For example: nl, en or fr |\n| `file` | Required
        | A CSV file formatted as a regular invitation CSV added as a HTTP POST file.
        |\n| `reminder` | Optional | Whether or not to send a reminder (1 means On,
        0 means Off). Defaults to 1 |\n\n### Example curl request\n```\ncurl -F \"file=@testCSV.csv\"
        https://api.starred.com/sendinvitations\\?company\\={{companyID}}\\&auth\\={{auth}}\\&form\\={{formId}}\\&from\\={{sender}}\\&template\\={{templateId}}\\&language\\={{language}}\n```"
      operationId: SendinvitationsCsvPost
      x-api-path-slug: sendinvitationscsv-post
      responses:
        200:
          description: OK
      tags:
      - Send
      - Invitation
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