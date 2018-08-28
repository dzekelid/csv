swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /dataset/import/{dataSetId}:
    post:
      summary: Import CSV
      description: Import a CSV into a DataSet
      operationId: dataSetImport
      x-api-path-slug: datasetimportdatasetid-post
      parameters:
      - in: formData
        name: csvImport_{dataSetColumnId}
        description: You need to provide dataSetColumnId after csvImport_, to know
          your dataSet columns Ids, you will need to use the GET /dataset/{dataSetId}/column
          call first
      - in: path
        name: dataSetId
        description: The DataSet ID to import into
      - in: formData
        name: files
        description: The file
      - in: formData
        name: ignorefirstrow
        description: flag (0,1), Set to 1 to Ignore first row, useful if the CSV file
          has headings
      - in: formData
        name: overwrite
        description: flag (0,1) Set to 1 to erase all content in the dataSet and overwrite
          it with new content in this import
      responses:
        200:
          description: OK
      tags:
      - Import
      - CSV