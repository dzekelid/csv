{
  "info": {
    "name": "import.io Get Extractor Extractorid Csv Latest",
    "_postman_id": "108425a5-d691-48cd-a34d-fe84d0437206",
    "description": "Get the latest crawl run results as a csv.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Extractor",
      "item": [
        {
          "id": "4e05fa7e-323c-4cc4-86a3-0a29e77e9081",
          "name": "getExtractorExtractorCsvLatest",
          "request": {
            "url": {
              "protocol": "http",
              "host": "schedule.import.io",
              "path": [
                "extractor/:extractorId/csv/latest"
              ],
              "variable": [
                {
                  "id": "extractorId",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the latest crawl run results as a csv."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f6ef7cbc-6b10-4375-8924-da7ecd862a1e"
            }
          ]
        }
      ]
    }
  ]
}