---
name: Starred
x-slug: starred
description: 'Better feedback for everyone, on a human scale. At Starred we like to
  work smart: working smarter to build great software, and working with smart companies
  who listen. As the feedback solution which puts the respondent first, we&rsquo;re
  empowering conversations between companies and their customers and employees. What&rsquo;s
  more, we equip them with the actionable insights they need to make better decisions
  and boost loyalty. With leading lights like Deliveroo, Heineken and Spotify already
  working with us to bring feedback to life, the road ahead for better feedback is
  looking good.'
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/starred-logo.png
x-kinRank: "7"
x-alexaRank: "916588"
tags: CSV
created: "2018-08-26"
modified: "2018-08-26"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/csv/master/_listings/starred/apis.md
specificationVersion: "0.14"
apis:
- name: Starred API - Send Invitation CSV
  x-api-slug: sendinvitationscsv-post
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
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/starred-logo.png
  humanURL: https://www.starred.com
  baseURL: https://example.com//
  tags: SaaS, Technology, internet, Relative Data, Service API, Feedback, Stars
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/csv/master/_listings/starred/sendinvitationscsv-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/csv/master/_listings/starred/sendinvitationscsv-post-openapi.md
- name: Starred API - Invitation Link CSV
  x-api-slug: invitationlinkscsv-post
  description: |-
    Generate links for users from a CSV file.

    **Request Parameters**

    | Parameter | Required | Description |
    | ------ | ------ | ------ |
    | `form` | Required | ID of the form that will be sent out |
    | `fromUserEmail` | Required | Email address of the sender |
    | `file` | Required | A CSV file formatted as a regular invitation CSV added as a HTTP POST file. |
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/starred-logo.png
  humanURL: https://www.starred.com
  baseURL: https://example.com//
  tags: SaaS, Technology, internet, Relative Data, Service API, Feedback, Stars
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/csv/master/_listings/starred/invitationlinkscsv-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/csv/master/_listings/starred/invitationlinkscsv-post-openapi.md
x-common:
- type: x-github
  url: https://github.com/starred-com
- type: x-twitter
  url: https://twitter.com/starred_com
- type: x-api-gallery
  url: http://standard.chartered.api.gallery.streamdata.io
- type: x-api-stack
  url: http://starred.stack.network
- type: x-blog
  url: https://www.starred.com/blog/
- type: x-crunchbase
  url: https://crunchbase.com/organization/starred
- type: x-email
  url: support@starred.com
- type: x-email
  url: legal@starred.com
- type: x-integrations
  url: https://www.starred.com/integrations/
- type: x-pricing
  url: https://www.starred.com/#
- type: x-website
  url: https://www.starred.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---