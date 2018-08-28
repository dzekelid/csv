swagger: "2.0"
x-collection-name: Import.io
x-complete: 1
info:
  title: import.io
  version: "1.0"
host: schedule.import.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /extractor/{extractorId}/csv/latest:
    get:
      summary: Get Extractor Extractorid Csv Latest
      description: Get the latest crawl run results as a csv.
      operationId: getExtractorExtractorCsvLatest
      x-api-path-slug: extractorextractoridcsvlatest-get
      parameters:
      - in: path
        name: extractorId
        description: the id of the extractor to start get the latest crawl run data
      responses:
        200:
          description: OK
      tags:
      - Extractor
      - ExtractorId
      - Csv
      - Latest