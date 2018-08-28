swagger: "2.0"
x-collection-name: Open Bank Project
x-complete: 1
info:
  title: Account and Transaction API Specification
  description: swagger-for-account-and-transaction-api-specification
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