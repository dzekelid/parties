---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Generates a correspondence to notify parties of a cancellation of
    a viewing.  Uses default values where possible.
  version: 1.0.0
  description: Generates a correspondence to notify parties of a cancellation of a
    viewing.  uses default values where possible..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/documentgeneration/offeraccepted:
    post:
      summary: Generates a correspondence any parties of the acceptance of an offer.  Uses
        default values where possible.
      description: Generates a correspondence any parties of the acceptance of an
        offer.  uses default values where possible..
      operationId: DocumentGeneration_OfferAcceptedLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationofferaccepted-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - Any
      - Parties
      - Of
      - Acceptance
      - Of
      - Offer
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/offerrejected:
    post:
      summary: Generates a correspondence any parties of the rejection of an offer.  Uses
        default values where possible.
      description: Generates a correspondence any parties of the rejection of an offer.  uses
        default values where possible..
      operationId: DocumentGeneration_OfferRejectedLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationofferrejected-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - Any
      - Parties
      - Of
      - Rejection
      - Of
      - Offer
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/offerwithdrawn:
    post:
      summary: Generates a correspondence to notify any parties of the withdrawl of
        an offer.  Uses default values where possible.
      description: Generates a correspondence to notify any parties of the withdrawl
        of an offer.  uses default values where possible..
      operationId: DocumentGeneration_OfferwithdrawnLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationofferwithdrawn-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Any
      - Parties
      - Of
      - Withdrawl
      - Of
      - Offer
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/completed:
    post:
      summary: Generates a correspondence to notify any parties of completion.  Uses
        default values where possible.
      description: Generates a correspondence to notify any parties of completion.  uses
        default values where possible..
      operationId: DocumentGeneration_CompletedLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcompleted-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Any
      - Parties
      - Of
      - Completion
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/exchanged:
    post:
      summary: Generates a correspondence to notify any parties of exchanged.  Uses
        default values where possible.
      description: Generates a correspondence to notify any parties of exchanged.  uses
        default values where possible..
      operationId: DocumentGeneration_ExchangedLetterPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationexchanged-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Any
      - Parties
      - Of
      - Exchanged
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/confirmationofviewing:
    post:
      summary: Generates a correspondence to notify all parties of a scheduled viewing.  Uses
        default values where possible.
      description: Generates a correspondence to notify all parties of a scheduled
        viewing.  uses default values where possible..
      operationId: DocumentGeneration_ConfirmationOfViewingPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationconfirmationofviewing-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - ""
      - Parties
      - Of
      - Scheduled
      - Viewing
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
  /api/documentgeneration/cancellationofviewing:
    post:
      summary: Generates a correspondence to notify parties of a cancellation of a
        viewing.  Uses default values where possible.
      description: Generates a correspondence to notify parties of a cancellation
        of a viewing.  uses default values where possible..
      operationId: DocumentGeneration_CancellationOfViewingPackBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationcancellationofviewing-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Correspondence
      - To
      - Notify
      - Parties
      - Of
      - Cancellation
      - Of
      - Viewing
      - ""
      - ""
      - Uses
      - Default
      - Values
      - Where
      - Possible
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