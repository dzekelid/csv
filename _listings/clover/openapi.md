---
swagger: "2.0"
x-collection-name: Clover
x-complete: 1
info:
  title: ""
  version: 1.0.0
host: /merchants
basePath: https://api.clover.com
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/merchants/{mId}/customers.csv:
    get:
      summary: Get a list of customers
      description: Gives information for every customer of a merchant by default.
      operationId: DelegatedGetCustomers
      x-api-path-slug: v3merchantsmidcustomers-csv-get
      parameters:
      - in: query
        name: expand
        description: 'Expandable fields: [addresses, emailAddresses, phoneNumbers,
          cards, metadata]'
      - in: query
        name: filter
        description: 'Filter fields: [id, firstName, lastName, fullName, customerSince,
          marketingAllowed, deletedTime, phoneNumber, emailAddress]'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Customers
      - Csv
  /v3/merchants/{mId}/shifts.csv:
    get:
      summary: Get .csv of all shifts
      description: Get .csv of all shifts.
      operationId: GetAllShiftsCSV
      x-api-path-slug: v3merchantsmidshifts-csv-get
      parameters:
      - in: query
        name: filter
        description: 'Filter fields: [id, employee'
      - in: path
        name: mId
        description: Merchant Id
      responses:
        200:
          description: OK
      tags:
      - Merchants
      - Shifts
      - Csv
---