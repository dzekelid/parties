---
swagger: "2.0"
x-collection-name: Open Bank Project
x-complete: 0
info:
  title: Open Bank Project Get Party
  description: Get Party
  termsOfService: https://www.openbanking.org.uk/terms
  contact:
    name: Service Desk
    email: ServiceDesk@openbanking.org.uk
  version: 1.0.0
basePath: /open-banking/v2.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /accounts/{AccountId}/party:
    get:
      summary: Get Account Party
      description: Get Party related to an account
      operationId: GetAccountParty
      x-api-path-slug: accountsaccountidparty-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Account
      - Party
  /party:
    get:
      summary: Get Party
      description: Get Party
      operationId: GetParty
      x-api-path-slug: party-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Banking
      - Banks
      - Party
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